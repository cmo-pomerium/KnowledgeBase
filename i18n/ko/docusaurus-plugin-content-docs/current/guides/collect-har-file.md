---
title: HAR 파일을 수집하는 방법
sidebar_position: 1
---

HAR 파일은 기술 지원 팀이 복잡한 문제를 해결하는 데 도움이 됩니다. 이러한 파일을 만들려면 Chrome 또는 Firefox를 사용하는 것이 좋습니다. 그러나 IE 11, Edge 및 Safari에서는 `.har` 파일 생성 및 내보내기 기능도 제공합니다.

## Chrome {#chrome}

Chrome에서 HAR 파일을 만들려면 다음을 수행합니다.

1. 문제가 발생한 URL로 이동합니다. 아직 문제를 재현하지 마세요.

2. ***개발자 도구***를 엽니다:

- 메뉴에서: ***메뉴 → 추가 도구 → 개발자 도구***.
- 키보드: ***Ctrl+Shift+C*** 또는 ***Ctrl+Alt+I***, Mac을 사용하는 경우 ***⌥+⌘+I***

3. ***네트워크 탭***을 클릭합니다.

4. 네트워크 탭의 왼쪽 상단에 있는 동그란 버튼을 찾아 빨간색 녹화 모드로 설정되어 있는지 확인합니다. 회색인 경우 클릭하여 빨간색으로 바꾸면 녹화가 시작됩니다.

5. ***지우기*** 버튼(기록 버튼 옆에 선이 그어진 원 버튼)을 사용하여 이전 활동을 모두 지웁니다.

6. 네트워크 탭에서 ***로그 보존*** 확인란을 선택합니다.

7. ***캐시 사용 안 함*** 확인란을 선택합니다.

![Chrome](https://cdn.adtidy.org/content/Kb/ad_blocker/guides/chrome.png)

8. 문제를 만드는 단계를 재현합니다.

9. 그리드를 마우스 오른쪽 버튼으로 클릭하고 ***콘텐츠가 포함된 HAR로 저장***을 선택하여 세션을 .har 파일로 저장합니다.

10. 문제에 대한 자세한 설명과 함께 AdGuard 지원팀(support@adguard.com)으로 전달하세요. 스크린샷을 첨부하는 것도 도움이 될 수 있습니다.

## Edge {#edge}

1. 문제가 발생한 URL로 이동합니다. 아직 문제를 재현하지 마세요.

2. ***개발자 도구***를 엽니다:

- 메뉴에서: ***메뉴 → 추가 도구 → 개발자 도구***.
- 키보드: ***Ctrl+Shift+C*** 또는 ***Ctrl+Alt+I***, Mac을 사용하는 경우 ***⌥+⌘+I***

3. ***네트워크 탭***을 클릭합니다.

4. 네트워크 탭의 왼쪽 상단에 있는 동그란 버튼을 찾아 빨간색 녹화 모드로 설정되어 있는지 확인합니다. 회색인 경우 클릭하여 빨간색으로 바꾸면 녹화가 시작됩니다.

5. ***지우기*** 버튼(기록 버튼 옆에 선이 그어진 원 버튼)을 사용하여 이전 활동을 모두 지웁니다.

6. 네트워크 탭에서 ***로그 보존*** 확인란을 선택합니다.

7. ***캐시 사용 안 함*** 확인란을 선택합니다.

![edge](https://cdn.adtidy.org/content/Kb/ad_blocker/guides/edge.png)

8. 문제를 만드는 단계를 재현합니다.

9. 그리드를 마우스 오른쪽 버튼으로 클릭하고 ***콘텐츠가 포함된 HAR로 저장***을 선택하여 세션을 .har 파일로 저장합니다.

10. 문제에 대한 자세한 설명과 함께 AdGuard 지원팀(support@adguard.com)으로 전달하세요. 스크린샷을 첨부하는 것도 도움이 될 수 있습니다.

## Firefox {#firefox}

Firefox에서 HAR 파일을 만들려면 다음을 수행합니다.

1. 문제가 발생한 URL로 이동합니다. 아직 문제를 재현하지 마세요.

2. ***네트워크*** 모드에서 개발자 도구를 엽니다:
- 메뉴에서: ***메뉴→웹 개발자→네트워크***.
- 키보드: ***Ctrl+Shift+C*** 또는 Mac을 사용하는 경우 **⌥+⌘+E**를 누릅니다.

3. 네트워크 탭의 왼쪽 상단에 있는 ***재생/일시 정지*** 버튼에 주목하세요.
- 버튼이 재생 모드에 있어야 합니다.

4. 현재 그리드에 정보가 표시되어 있는 경우 재생/일시 정지 버튼 옆에 있는 ***휴지통 삭제*** 버튼을 클릭하여 지웁니다.

5. 네트워크 탭에서 ***로그 유지*** 확인란을 선택합니다.

6. ***캐시 사용 안 함*** 확인란을 선택합니다.

![파이어폭스](https://cdn.adtidy.org/content/Kb/ad_blocker/guides/firefox.png)

7. 문제를 만드는 단계를 재현합니다.

8. 그리드를 마우스 오른쪽 버튼으로 클릭하고 ***모두 HAR로 저장***을 선택하여 세션을 .har 파일로 저장합니다.

9. 문제에 대한 자세한 설명과 함께 AdGuard 지원팀(support@adguard.com)으로 전달하세요. 스크린샷을 첨부하는 것도 도움이 될 수 있습니다.

## Internet Explorer 11 {#ie11}

Internet Explorer 11에서 HAR 파일을 만들려면 다음을 수행합니다.

1. 문제가 발생한 URL로 이동합니다. 아직 문제를 재현하지 마세요.

2. ***네트워크*** 모드에서 개발자 도구를 엽니다:
- 도구 톱니바퀴 메뉴에서: ***개발자 도구*** → ***네트워크 탭***.
- 키보드: ***F12→네트워크*** 탭.

3. 프로파일링 세션 시작 ***재생*** 버튼과 프로파일링 중지 ***중지*** 버튼이 네트워크 탭 왼쪽 상단에 있습니다.
- 녹화 중 재생 버튼은 회색으로 표시되고 중지 버튼은 빨간색으로 표시됩니다. ***에 들어가*** 모드를 재생합니다.

4. 네트워크 탭의 ***세션 지우기*** 버튼을 사용하여 아래쪽 그리드에 표시되는 세션 정보를 모두 지웁니다. 아이콘 위로 마우스를 가져가면 이름을 볼 수 있습니다.
- ***세션 지우기*** 버튼은 세 줄 아이콘에 X가 표시되어 있습니다.

5. ***캐시 사용 안 함*** 확인란을 선택합니다.

6. 문제를 만드는 단계를 재현합니다.

7. 네트워크 탭에서 ***디스크 저장*** 버튼(HAR로 내보내기)을 클릭하여 세션을 .har 파일로 저장합니다.

8. 문제에 대한 자세한 설명과 함께 AdGuard 지원팀(support@adguard.com)으로 전달하세요. 스크린샷을 첨부하는 것도 도움이 될 수 있습니다.

## Safari {#safari}

Safari에서 HAR 파일을 만들려면 다음을 수행합니다.

1. 화면 상단의 Safari 메뉴 표시줄에서 ***개발*** 메뉴를 확인합니다. ***메뉴 표시줄에 개발 메뉴 표시***옆의 하단에 있는 확인란을 선택합니다.
- 표시되지 않으면 ***Safari→환경설정→고급***으로 이동하여 켜십시오.

2. 문제가 발생한 URL로 이동합니다. 아직 문제를 재현하지 마세요.

3. 웹 인스펙터에서 ***네트워크*** 탭을 엽니다:
- 메뉴에서: ***개발→웹 검사기 표시→네트워크***.
- 키보드: ***⌥+⌘+I→네트워크***

4. 네트워크 탭의 오른쪽에 있는 ***로그 보존*** 확인란을 선택합니다.

5. 네트워크 탭의 맨 오른쪽에 있는 ***휴지통 삭제*** 아이콘을 클릭하여 현재 네트워크 항목을 지웁니다.

6. ***캐시 사용 안 함*** 확인란을 선택합니다.

7. 문제를 만드는 단계를 재현합니다.

8. ***내보내기*** 아이콘 옆의 ***로그 보존***을 클릭하여 세션을 .har 파일로 저장합니다.

9. 문제에 대한 자세한 설명과 함께 AdGuard 지원팀(support@adguard.com)으로 전달하세요. 스크린샷을 첨부하는 것도 도움이 될 수 있습니다.

## Android {#android}

To create HAR files, follow these steps:

1. AdGard를 열고 ***설정***으로 이동합니다.

2. 메뉴에서 ***고급*** 을 선택합니다.

3. ***낮은 레벨 설정***을 선택합니다.

4. `pref.har.capture`를 활성화합니다(보호 기능을 다시 시작해야 합니다).

5. 이제 문제를 재현하여 앱을 열고 광고가 표시되도록 필요한 작업을 수행합니다.

6. 이제 `pref.har.capture`을 다시 끕니다.

7. 돌아가서 ***로그 및 시스템 정보 내보내기*** → ***저장***을 탭합니다.

## Windows {#windows}

1. ***설정*** → ***일반 설정*** → ***고급 설정** 을 열고 아래로 스크롤합니다.

2. ***HAR 쓰기 활성화*** 확인란을 선택합니다.

3. 문제를 재현합니다.

4. ***일반 설정*** → ***로그 내보내기*** → ***저장***으로 이동합니다.

5. 해당 확인란을 선택 취소하여 HAR 쓰기를 비활성화합니다.
