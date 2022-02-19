- 플러터 프로젝트 생성: `flutter create [프로젝트명]`</br>
- 플러터 실행: `flutter run`</br>
- iOS 에뮬레이터 실행: `open -a Simulator`</br>
- 안드로이드 에뮬레이터 리스트 조회: `emulator -list-avds`</br>
- 안드로이드 에뮬레이터 실행: `emulator -avd@[프로젝트명]` or `emulator -avd [프로젝트명]`</br>

안드로이드 에뮬레이터 리스트 조회시 아무 리스트가 조회되지 않을 경우

> 안드로이드 스튜디오 실행 -> device manager -> create device

안드로이드 에뮬레이터 설치 후 첫 실행시

> vscode => command + shift + p => Flutter: Select Device

- lint 적용1: `dart pub add --dev lints` after `pub get`
- lint 적용2: `flutter pub add --dev flutter_lints` after `pub get`

- development
  flutter run --target lib/main_development.dart
- production
  flutter run --target lib/main_production.dart

- flutter_launcher_icons-development.yaml setting
- flutter_launcher_icons-production.yaml setting

- cmd run 이미지 생성(production, development)
  flutter pub run flutter_launcher_icons:main -f flutter_launcher_icons\*
