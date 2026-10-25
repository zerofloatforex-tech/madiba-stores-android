# Madiba Stores Android wrapper

This Android Studio project packages the live website https://www.madibastores.com/ in an Android WebView. It does not create a separate database: logins, stock, sales, invoices, and reports continue to use the same hosted website/backend, so changes made on the web are shared with the app.

## Build an installable APK
1. Install Android Studio on a Windows/Mac/Linux computer.
2. Extract this ZIP and open the `MadibasStoresAndroid` folder in Android Studio.
3. Allow Gradle sync and install the Android SDK Platform 35 if prompted.
4. Select **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
5. When complete, select **locate** in the notification. The APK is normally at `app/build/outputs/apk/debug/app-debug.apk`.
6. Transfer `app-debug.apk` to your Android phone, open it, and allow installation from that file source if Android asks.

## Important
- Internet access is required; this app displays the live hosted website rather than storing a separate copy of the store database.
- The website must be reachable over HTTPS and its login/session flows must work in Android WebView.
- If your website uses a payment, PDF, camera, barcode-scanning, or file-upload flow, test those on the phone; some flows may need extra native integration.
- This ZIP is the Android Studio source project, not a compiled APK. A build machine with Android SDK/Gradle is required to generate the APK.
