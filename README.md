# DGCalendar

Google Calendar와 Google Tasks를 바탕화면에서 확인하고 관리하는 Windows 달력입니다. Google 계정을 연결하거나, 로그인 없이 로컬 일정과 할 일을 사용할 수 있습니다.

[홈페이지](https://dgcalendar.remerer.chatgpt.site/) · [최신 릴리스](https://github.com/remerer/DGCalendar-releases/releases/latest) · [문제 신고·개선 요청](https://github.com/remerer/DGCalendar-releases/issues/new/choose)

![DGCalendar 월간 달력 예시](docs/images/calendar-example.png)

예시 일정과 할 일을 넣은 실제 앱 화면입니다. 배경 밝기·투명도·요일 색·글자 크기를 조절할 수 있습니다.

## 주요 기능

- 월간 달력에서 일정·할 일 확인, 등록, 편집, 삭제와 할 일 완료 처리
- Google Calendar·Tasks 연동과 표시할 캘린더 선택
- 인터넷이나 Google 연결 없이 사용하는 로컬 일정·할 일
- 날짜의 빈 공간을 더블클릭하는 빠른 입력
- 투명도·배경 밝기·요일 색·글자 크기와 굵기 설정
- 창 이동·크기 조절과 잠금, 여러 모니터 지원, Windows 시작 시 실행
- 선택한 캘린더의 기념일 표기와 공휴일 강조

Windows 표시 언어가 한국어이면 한국어로, 그 외에는 영어로 표시합니다.

## 다운로드와 첫 실행

**Windows 10 1809 이상 또는 Windows 11 · x64** 환경에서 사용할 수 있습니다.

**기본 버전을 권장합니다.** 두 버전의 기능은 같습니다.

| 버전 | 다운로드 | 선택 안내 |
|---|---|---|
| **권장 · 기본 버전** | [DGCalendar v0.1.3](https://github.com/remerer/DGCalendar-releases/releases/download/v0.1.3/DGCalendar-0.1.3-win-x64.zip) | PC에 따라 Microsoft 공용 구성요소의 추가 설치가 필요할 수 있습니다. |
| 추가 설치를 줄인 버전 | [DGCalendar v0.1.3 · 구성요소 포함](https://github.com/remerer/DGCalendar-releases/releases/download/v0.1.3/DGCalendar-0.1.3-win-x64-static-crt.zip) | 기본 버전의 구성요소를 설치하기 어려운 경우 선택하세요. |

1. ZIP을 다운로드해 **전체 압축 해제**합니다.
2. `DGCalendar` 폴더 안의 `DGCalendar.exe`를 실행합니다. 별도의 앱 설치 과정은 없습니다.
3. Google 연동을 사용하려면 **설정 → 계정 → Google 연결**에서 로그인하고 Calendar·Tasks 권한을 허용한 뒤, 표시할 캘린더를 선택합니다.

Google 연동에는 별도의 API 설정이 필요하지 않습니다.

Google Calendar·Tasks 접근 권한 검증은 **신청 후 심사 중**입니다. 승인 전에는 Google 로그인 시 미검증 앱 안내와 사용자 수 제한이 적용될 수 있습니다.

기본 버전에서 Microsoft 구성요소 설치를 요구하면 [Microsoft 공식 안내](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist)의 **X64** 패키지를 설치해 주세요. 실행에 필요한 파일이 함께 있으므로 압축을 푼 폴더 전체를 유지해 주세요.

## 기본 사용법

| 하고 싶은 일 | 조작 |
|---|---|
| 일정·할 일 등록 | 상단 `+` 또는 날짜의 빈 공간 더블클릭. 더블클릭 동작은 설정에서 선택합니다. |
| 상세 보기·편집·삭제 | 항목을 클릭해 상세 보기를 열고, 연필 또는 휴지통 버튼을 사용합니다. |
| 할 일 완료·해제 | 항목 왼쪽의 체크 영역을 클릭합니다. |
| 창 이동·크기 조절 | 잠금을 해제하고 상단 바 또는 창 테두리를 드래그합니다. |
| 모양·계정·기념일 설정 | 달력의 설정 버튼 또는 트레이 아이콘 메뉴를 엽니다. |

## 새 버전 알림

**설정 → 앱 정보**에서 현재 버전과 새 버전을 확인하고, 새 버전 알림을 켤 수 있습니다. 업데이트 파일은 GitHub에서 직접 내려받습니다.

새 버전으로 바꿀 때는 앱을 트레이 메뉴에서 종료하고, 새 ZIP을 **새 폴더**에 압축 해제해 실행하세요. 기존 일정과 설정은 유지됩니다. Windows 시작 시 실행을 사용 중이면 새 폴더에서 해당 옵션을 다시 켜 주세요.

## 문의와 후원

- [문제 신고·개선 요청](https://github.com/remerer/DGCalendar-releases/issues/new/choose): 양식을 선택하면 입력 안내를 볼 수 있습니다.
- [Buy Me a Coffee](https://buymeacoffee.com/remerer): 앱의 **설정 → 앱 정보**에서도 커피 아이콘으로 열 수 있습니다.
- [개인정보처리방침](https://dgcalendar.remerer.chatgpt.site/privacy.html)

<details>
<summary>개발 및 배포 정보</summary>

- DGCalendar는 Desktop with Google Calendar의 약자입니다. 이 저장소는 배포 파일과 사용 안내를 제공합니다.
- 기본 버전은 동적 CRT를 사용하며 Microsoft Visual C++ v14 x64 재배포 가능 패키지가 필요할 수 있습니다. 대체 버전은 Rust 코어에 CRT를 정적으로 연결해 추가 설치 필요를 줄입니다.
- 두 버전 모두 .NET과 Windows App SDK 런타임을 포함합니다. 실행 파일만 따로 옮기거나 두 버전의 파일을 섞지 마세요.
- 일정·할 일·설정은 `%LOCALAPPDATA%\CalendarDesktop`에 보관합니다. Google 토큰과 일정 데이터는 Windows 사용자에 묶여 암호화됩니다.
- 배포 파일에는 공용 Google Desktop OAuth 앱 설정을 포함하며, 개인 로그인 토큰과 일정 데이터는 포함하지 않습니다.
- 현재 배포에는 코드 서명이 없어 Windows에서 게시자를 확인하지 못할 수 있습니다.

</details>

DGCalendar는 Google 또는 Microsoft의 공식 제품이 아닌 독립 앱입니다.
