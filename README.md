# Description

Use GitHub Actions workflow to disable FLAG_SECURE for APK/APKS/XAPK, etc, via LSPatch.

In simpler terms, this disables screen mirroring protection of the app, so that you can use applications like Scrcpy to screen mirror the app, which would otherwise appear as a black screen.

To use it, you need to use the GitHub Actions workflow system -

1. [Fork](https://github.com/George-Seven/lspatch_disable_flag_secure/fork) this repo
2. Goto "Actions" tab at the top of the page
3. Enable workflows
4. Select drop down menu "All workflows"
5. Select "Rebuild APK with Disable FLAG_SECURE"
6. Select "Run workflow"
7. There are two choices for selecting apk, either use package name of app (eg:- `com.naver.linewebtoon`) or a direct link to the apk. Fill the corresponding field.
8. Scroll down and select the green "Run workflow" button.
9. Wait some seconds until the build finishes with a green tick.
10. Refresh the page once to sync
11. Scroll down and download the `patched-apk` zip.
12. Unzip it and use the patched apk.

That's about as detailed as can be.

Remember to uninstall the old app before installing the patched apk.
