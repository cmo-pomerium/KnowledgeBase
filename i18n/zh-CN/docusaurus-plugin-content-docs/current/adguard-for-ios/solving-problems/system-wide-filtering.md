---
title: 如何在 AdGuard iOS 版设置系统层面的过滤？
sidebar_position: 2
---

:::info

This article covers AdGuard for iOS, a multifunctional ad blocker that protects your device at the system level. To see how it works, [download the AdGuard app](https://adguard.com/download.html?auto=true)

:::

## 关于系统层面上的过滤

系统层面上的过滤是指不仅在 Safari 浏览器里，而且在其它应用程序和浏览器里屏蔽广告及跟踪器。 这篇文章的内容讲述如何在您的 iOS 设备上设置系统层面的广告拦截。

在 iOS 上，仅有一个方式允许我们在系统层面上拦截广告和跟踪器，就是使用 [DNS 过滤](https://adguard-dns.io/kb/general/dns-filtering/)。 首先，您需要启用 DNS 保护。 以启用 DNS 保护，请打开 *AdGuard iOS 版的设置* → 启用*「DNS 保护」*。

![DNS 保护屏幕 *mobile_border](https://cdn.adtidy.org/public/Adguard/Blog/ios_dns_protection.PNG)

到了这一步，如您的目标是在系统层面上拦截广告和跟踪器，那么您有两个选择：

1. 启用 AdGuard DNS 服务器（*「设置」* →*「DNS 保护」* →*「DNS 服务器」* → *「AdGuard DNS」*）。
2. 添加能够拦截广告和跟踪网域的 DNS 过滤器/hosts 文件，就是 AdGuard DNS 过滤器。

虽然第二个选择需要花更长时间设置，但是这个选择具有以下几个优点：

* 您可亲自选择任何 DNS 服务器，并不需要使用某一个特定的拦截服务器。
* 您可以同时添加几个 DNS 过滤器和/或 Hosts 文件，但是您不能同时使用几个 DNS 服务器。

![DNS 过滤工作原理](https://cdn.adtidy.org/public/Adguard/kb/DNS_filtering/how_dns_filtering_works_en.png)

## 如何添加 DNS 过滤器/Hosts 文件

您可以添加任何一个 DNS 过滤器或 Hosts 文件。无论是 DNS 过滤器还是 Hosts 文件，说明的内容都是一样的。 比如，让我们一起尝试添加 [AdGuard DNS 过滤器](https://github.com/AdguardTeam/AdguardSDNSFilter)。 AdGuard DNS 过滤器是由几个过滤器（包括 AdGuard 基础过滤器、社交媒体过滤器、防跟踪保护过滤器、移动广告过滤器、EasyList、EasyPrivacy 等等）组成的。为了使该过滤器与 DNS 级广告拦截的兼容性更佳，我们特地简化了它。

1. 打开 *AdGuard iOS 版的设置* → *「通用」*。
2. 启用**高级模式**。 「*高级设置*」标签将出现。 打开它。

![打开 AdGuard 设置并启用高级模式 *mobile_border](https://cdn.adtidy.org/public/Adguard/Release_notes/iOS/v4.0/advanced_mode_en.jpg)

![高级设置屏幕 *mobile_border](https://cdn.adtidy.org/public/Adguard/Blog/ios_advanced_settings.PNG)

:::note

We don't recommend touching other settings you'll find inside the *Advanced settings* tab, especially when it comes to *Low-level settings*. 有些设置可能会导致互联网连接中断或会造成您的隐私安全被泄露，因此您要保持警惕。 下面的内容讲述的是，为了添加 AdGuard DNS 过滤器需要进行的步骤。

:::

3. 请复制此链接：`https://raw.githubusercontent.com/AdguardTeam/FiltersRegistry/master/filters/filter_15_DnsFilter/filter.txt`（这是 AdGuard DNS 过滤器的链接）。
4. 打开 *AdGuard iOS 版的设置* → *「DNS 保护」* → *「DNS 过滤」*（仅在*高级模式*开启时使用）→*「DNS 过滤器」*。
5. Tap *Add a filter*, paste the link into the filter URL field, and tap 'Next'.

![添加 DNS 过滤器屏幕 *mobile_border](https://cdn.adtidy.org/public/Adguard/Blog/ios_adding_a_filter.PNG)

通过在第三步粘贴另一个链接，您就可以使用同样的方式添加任何其它的 DNS 过滤器。 [在这里](https://filterlists.com)您可以找到各种过滤器以及它们的链接。
