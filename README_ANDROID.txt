RISE OF THE DEMON KING — ANDROID APK BUILD

This project includes the playable game and an automated GitHub Actions workflow.
The ZIP itself is NOT an APK.

EASIEST BUILD METHOD (uses GitHub's cloud runner):
1. Sign in to GitHub and create a new empty repository, e.g. RiseOfDemonKing.
2. Upload the contents of this project ZIP to the repository's main branch. Make sure
   settings.gradle, build.gradle, app/, and .github/ are at the repository root.
3. Open the repository's Actions tab.
4. Select "Build Android APK" and press "Run workflow" if it has not started automatically.
5. Wait for the run to finish successfully.
6. Open the completed workflow run and download the artifact named
   RiseOfDemonKing-debug-apk.
7. Extract the downloaded artifact ZIP; inside is app-debug.apk.
8. Transfer/open app-debug.apk on your Android phone and follow Android's install prompts.

BUILD LOCALLY:
1. Open this project folder in Android Studio on a computer.
2. Let Gradle sync and install Android SDK Platform 35 if requested.
3. Select Build > Build Bundle(s) / APK(s) > Build APK(s).
4. APK output: app/build/outputs/apk/debug/app-debug.apk.

GAME NOTES:
- The game is bundled locally in app/src/main/assets/index.html and does not need internet.
- The Android wrapper uses WebView, with JavaScript and DOM storage enabled.
- This is a debug APK, suitable for testing, not a Play Store release.
- A computer is not required for GitHub's cloud build, but uploading project files and
  downloading the APK artifact through GitHub may be easier in desktop mode.
