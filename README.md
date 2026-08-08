# JARVIS Android

Package: `com.jarvis.assistant`

- Kotlin Android project.
- SpeechRecognizer, русский язык.
- TextToSpeech, русский язык.
- Ровно 1500 уникальных локальных русских фраз: `app/src/main/assets/phrases.json`.
- Тёмный интерфейс, реактор, анимация прослушивания.
- Intent-команды: YouTube, браузер, музыка, настройки, сведения об устройстве.
- Время и дата вычисляются локально.
- Базовые ответы не требуют внешнего ИИ API.

Откройте проект в Android Studio → Gradle Sync → Build → Build APK(s).

«Выключись» завершает голосовое прослушивание JARVIS, а не выключает телефон.


## Сборка APK без ПК через GitHub

1. Создайте пустой репозиторий на GitHub.
2. Загрузите в него содержимое этой папки вместе с `.github/workflows/build-apk.yml`.
3. Откройте вкладку **Actions**.
4. Выберите **Build JARVIS APK**.
5. Нажмите **Run workflow**.
6. После завершения откройте готовый workflow и найдите раздел **Artifacts**.
7. Скачайте `JARVIS-debug-APK`.
8. Внутри будет `app-debug.apk`.

GitHub выполняет сборку на своём сервере, поэтому Android Studio на телефоне не нужна.
