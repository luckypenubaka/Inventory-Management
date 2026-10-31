INVENTORY MANAGER - ANDROID APP PROJECT
=======================================

Features
--------
- Dashboard showing product count, total units, and low-stock count
- Add product with name, category, quantity, price, and low-stock threshold
- Search products by name or category
- Adjust stock by entering a positive or negative quantity
- Delete products with confirmation
- SQLite local database; product data remains after closing/reopening the app
- Works offline; no login or internet required

BUILD THE APK USING ANDROID STUDIO
----------------------------------
1. Install Android Studio from https://developer.android.com/studio
2. Extract InventoryManagementApp.zip to a folder.
3. Open Android Studio -> Open -> select the extracted InventoryManagementApp folder.
4. Allow Gradle sync to finish. If prompted, install Android SDK Platform 35 and use JDK 17.
5. To test, connect an Android phone with USB debugging enabled or create an emulator, then press Run.
6. To create an APK: Build -> Build Bundle(s) / APK(s) -> Build APK(s).
7. When the build completes, click "locate" in the notification.
   The debug APK is usually at:
   app/build/outputs/apk/debug/app-debug.apk
8. Transfer app-debug.apk to your phone and open it to install. You may need to allow
   installation from that file manager. Only install APKs you built or trust.

PROJECT STRUCTURE
-----------------
app/src/main/java/com/bytexl/inventory/MainActivity.java
    App interface, forms, search, product cards, stock adjustment and dashboard.
app/src/main/java/com/bytexl/inventory/DatabaseHelper.java
    SQLite database and product data operations.
app/src/main/AndroidManifest.xml
    Android app entry point and app label.
app/src/main/res/values/styles.xml
    Basic app theme.
app/build.gradle
    Android build settings.

TECHNOLOGY
----------
Java, Android SDK, SQLite.

NOTES
-----
- This is a student project starter. Test the app on your target phone before presenting it.
- Data is stored locally on the phone. It is not shared across multiple devices.
- The app currently supports adding, searching, adjusting stock, and deleting products.
- Edit-product functionality, login, export reports, and cloud sync are not included in this version.
