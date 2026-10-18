# DGCalendar

Desktop with Google Calendar. 일정과 할 일을 날짜별로 보여주는 Windows 바탕화면 달력입니다.

이 저장소는 **Windows 배포 파일과 릴리스 안내**를 제공합니다. 소스 코드는 포함하지 않습니다.

첫 배포본을 준비 중입니다. 정식 릴리스가 공개되면 아래 다운로드 링크에서 받을 수 있습니다.

## 다운로드와 실행

1. [최신 릴리스](https://github.com/remerer/DGCalendar-releases/releases/latest)에서 `DGCalendar-버전-win-x64.zip`을 받습니다.
2. ZIP 전체를 원하는 폴더에 압축 해제합니다. EXE만 따로 옮기면 실행에 필요한 런타임과 화면 리소스를 찾을 수 없습니다.
3. 압축 해제된 `DGCalendar` 폴더에서 `DGCalendar.exe`를 실행합니다.

지원 대상은 **Windows 10 1809 이상 / Windows 11, x64**입니다. .NET과 Windows App SDK 런타임을 포함하는 배포입니다. 이전 Windows 버전과 ARM64 기본 실행은 지원하지 않습니다. Windows 최소 버전은 빌드 설정의 하한이며 모든 Windows 빌드에서의 실기 검증을 뜻하지 않습니다.

**Microsoft Visual C++ v14 재배포 가능 패키지(x64)**가 필요합니다. PC에 설치되어 있지 않거나 `VCRUNTIME140.dll` 누락 안내가 나오면 [Microsoft 공식 다운로드 안내](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist)를 통해 x64 패키지를 설치해 주세요.

초기 시험 배포에는 코드 서명이 없습니다. Windows가 게시자를 확인하지 못하거나 SmartScreen 안내를 표시할 수 있습니다. 다운로드한 ZIP은 같은 릴리스의 `SHA256SUMS.txt`로 무결성을 확인할 수 있습니다.

## 주요 기능

- 바탕화면 월간 달력과 일정·할 일 등록, 편집, 삭제, 완료 처리
- Google 연결 없이 사용할 수 있는 독립 로컬 저장
- 선택한 Google Calendar와 Google Tasks 연동
- 날짜 빈 공간을 더블클릭해 빠르게 입력
- 투명도·배경 밝기·요일 색·글자 크기와 굵기 조절
- 위치·크기 잠금, 여러 모니터 지원, Windows 시작 시 실행 옵션
- 선택한 캘린더의 기념일 이름과 공휴일 강조 표시

## Google 연결 안내

공개 ZIP에는 OAuth 클라이언트 설정이나 사용자 인증 정보를 포함하지 않습니다. 따라서 **새 PC에서는 로컬 기능을 바로 사용**할 수 있으며, Google 로그인에는 배포자의 Desktop OAuth 클라이언트 설정 제공이 별도로 필요합니다. 이미 이 PC에 저장된 Google 설정과 토큰은 앱 업데이트 시 유지됩니다.

Google 로그인 제공 범위는 릴리스 안내를 확인해 주세요. 배포자의 Google OAuth 게시·검증 상태와 테스트 사용자 제한은 이 저장소만으로 확인할 수 없습니다. 사용자의 비밀번호를 앱에 입력하는 방식은 사용하지 않습니다.

## 업데이트

앱 옵션의 GitHub 링크에서 릴리스와 변경 내용을 확인할 수 있습니다. 앱은 새 정식 릴리스를 확인해 알리며 자동 설치하지 않습니다. 직접 업데이트하려면 앱을 트레이 메뉴에서 종료하고 새 ZIP을 **새 폴더**에 압축 해제한 뒤 실행합니다. 시작 프로그램을 사용 중이라면 새 폴더에서 해당 옵션을 다시 켜 경로를 갱신합니다.

일정·할 일·설정은 앱 폴더와 별도로 현재 사용자의 `%LOCALAPPDATA%\CalendarDesktop`에 보관합니다. Google 토큰과 일정 데이터는 Windows 사용자에 묶여 암호화되므로 다른 PC나 Windows 계정으로 파일을 복사하는 방식의 이전은 지원하지 않습니다.

GitHub 계정으로 저장소의 **Watch → Custom → Releases**를 설정하면 GitHub에서도 새 릴리스 알림을 받을 수 있습니다.

## 피드백과 후원

문제 제보: [Issues](https://github.com/remerer/DGCalendar-releases/issues)

계정 정보, OAuth JSON, 토큰, 개인 일정, 앱의 암호화 저장 파일을 공개 이슈에 첨부하지 마세요.

개발 후원: [Buy Me a Coffee](https://buymeacoffee.com/remerer)

DGCalendar는 독립 앱이며 Google 또는 Microsoft의 공식 제품이 아닙니다.
