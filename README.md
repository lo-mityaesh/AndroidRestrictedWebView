# Android Restricted WebView

The Android Restricted WebView is an Android application template that allows you to display a specific website using a WebView while restricting access to other sites. If the application attempts to load a URL other than the allowed site, an error message "This URL is not allowed" will be displayed.

## Configuration

To configure the application and set the allowed website, follow these steps:

1. Open the project in Android Studio.
2. Navigate to the `MainActivity.java` file.
3. Locate the line 33 containing the `ALLOWED_URL` constant.
4. Replace the value of the `ALLOWED_URL` constant with the desired URL for the allowed site.
   ```java
   private static final String ALLOWED_URL = "www.example.com";
   ```
5. Save the changes.

Make sure to provide a valid URL for the website you want to allow in the application.

## Portrait Mode Configuration

The Android Restricted WebView also allows for the forcing of screen orientation to portrait mode. This is controlled by the `FORCE_PORTRAIT` constant on line 31 in the `MainActivity` class.

To configure this, follow these steps:

1. In the `MainActivity.java` file, locate the line 34 containing the `FORCE_PORTRAIT` constant.
2. Replace the value of the `FORCE_PORTRAIT` constant to `true` to enforce portrait mode or `false` to allow the system and user preferences to determine the screen orientation.
   ```java
   private static final boolean FORCE_PORTRAIT = true; // Change this value to true or false
   ```
3. Save the changes.

After modifying this value, you need to recompile and redeploy the application for the change to take effect.

## Changing the Package Name

To change the package name of the application, follow these steps:

1. Open the project in Android Studio.
2. Locate the `build.gradle` file (Module: app).
3. In the `build.gradle` file, find the line 9 containing the `applicationId`.
4. Replace the value of the `applicationId` with the desired package name.
   ```gradle
   defaultConfig {
       // ...
       applicationId "com.example.newpackagename"
       // ...
   }
   ```
5. Sync the project with Gradle to apply the changes.

Ensure that the new package name follows the proper naming conventions.

## Usage

After configuring the allowed URL, setting the portrait mode preference, and optionally changing the package name, you can run the application on an Android emulator or device. The application will display the web page of the allowed site within the WebView.

If an attempt is made to load a URL other than the allowed site, the application will display an error message "This URL is not allowed" instead of the content.


## License

This application is distributed under the GNU General Public License version 3 (GNU GPL-3.0). See the [LICENSE](LICENSE) file for more details.

## Disclaimer

Please note that I am not a lawyer and the information provided here should not be considered legal advice. It is important to consult with a qualified legal professional to ensure compliance with all relevant licensing requirements and obligations.

## Support Me
[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/J3J6N3QW7)
