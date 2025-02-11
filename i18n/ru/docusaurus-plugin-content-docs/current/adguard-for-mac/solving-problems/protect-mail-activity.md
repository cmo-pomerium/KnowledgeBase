---
title: Защитой конфиденциальности в Почте и AdGuard
sidebar_position: 8
---

:::info

В этой статье рассказывается об AdGuard для Mac — многофункциональном блокировщике рекламы, который защищает ваше устройство на системном уровне. Чтобы увидеть, как он работает, [скачайте приложение AdGuard](https://adguard.com/download.html?auto=true)

:::

## В двух словах

Приложение Почта Apple теперь использует прокси-сервер для скрытия IP-адреса пользователя при загрузке изображений из электронных писем.

![Защита конфиденциальности в Почте](https://cdn.adtidy.org/content/kb/ad_blocker/mac/mac_protectMailActivity.jpg)

Но эта функция не работает при наличии активного VPN-соединения. Поскольку AdGuard рассматривается Почтой Apple как VPN, изображения не загружаются автоматически.

Apple комментирует эту проблему [здесь](https://support.apple.com/HT212797).

## Подробное описание проблемы

AdGuard для Mac теперь использует встроенный в macOS механизм фильтрации сокетов на основе network extensions API. Этот новый и довольно глючный механизм заменил старые добрые расширения Kernel. За последние полтора года мы сообщили Apple более чем о 20 (!) ошибках, связанных с новым методом фильтрации.

Network extensions API имеет VPN-подобную конфигурацию со списком записей типа route. На Big Sur мы использовали правила split-tunnel, чтобы избежать создания правила default route, поскольку оно вызывало проблемы в ранних версиях Big Sur. Эти проблемы были решены в Monterey, поэтому ничто не мешает нам использовать правило default route.

На Monterey появилась функция iCloud Private Relay. Функции конфиденциальности в приложении Почта также используют серверы iCloud Private Relay.

В результате AdGuard не может работать вместе с iCloud Private Relay и функциями конфиденциальности приложения Почта:
1. iCloud Private Relay применяется к соединениям на уровне библиотек — до того, как они достигают уровня сокета, где работает AdGuard.
2. iCloud Private Relay использует QUIC, который AdGuard не может блокировать, поскольку фильтрация HTTP/3 пока не доступна.
3. Поэтому AdGuard блокирует QUIC, включая и трафик iCloud Private Relay — иначе блокировка рекламы невозможна.
4. При использовании iCloud Private Relay и переключении AdGuard в режим "split-tunnel" невозможно открыть сайты в Safari.
5. Чтобы обойти эту проблему для Monterey, мы применяем правило "default route". Тогда Private Relay видит это правило, он автоматически отключается. Таким образом, AdGuard работает без проблем на Monterey, но iCloud Private Relay отключается.

`network.extension.monterey.force.split.tunnel` восстанавливает поведение Big Sur, но этот вариант может нарушить доступ к сайтам из-за (3) и (4). Мы продолжаем искать решение этой проблемы. Один из вариантов — внедрить HTTP/3-фильтрацию.

## Рекомендуемое решение
Мы рекомендуем использовать более традиционный VPN-сервис, такой как [AdGuard VPN](https://adguard-vpn.com/), вместо новых функций конфиденциальности Apple.
