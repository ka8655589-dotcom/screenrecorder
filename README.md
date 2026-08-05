Minimal ScreenRecorder sample (for CI build)

This repo contains a minimal Android app so GitHub Actions can build an APK for you to download.
The app is just a placeholder activity (no recording code). After you get the APK working, we can add the full recording + Drive upload code.

How to get the APK:
1. Commit these files to the `main` branch (they should already be added).
2. Open the repository on GitHub and click the Actions tab.
3. Click the workflow run "Android CI - Build APK" and wait for it to finish.
4. When successful, download the artifact `app-debug-apk` from the run page.
5. Inside the ZIP find `app/build/outputs/apk/debug/app-debug.apk` — install it on your phone (allow installs from unknown sources).

If the build fails, open the failing step logs (Actions → run → job → failing step), copy the first ~40 lines of the error, and paste them in chat so I can help debug.
