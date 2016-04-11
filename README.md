# Crash-Reporter
Easily get your Android App crash reports to your E-mail

# Features:
Get a Full report of crash data of UnHandled Exception.

# Installation steps:
1.	Download the Jar File.
2.	Add it to your Android project libs (Copy&Paste or dragging).
**make sure to right click --> add as library.

![ScreenShot](https://raw.github.com/Dgotlieb/Crash-Reporter/master/addJar.png)

3.	Call it from any Context (e.g: Activity/Fragment/Services/Receivers and etc), 
    by sending 4 parameters: Context, Sender, Password and recipients.

ExceptionHandler.init(this, "user@gmail.com", "123456","recipients@gmail.com");

4. Don't forget to add Manifest.xml permissions, as following:

uses-permission android:name="android.permission.INTERNET"*

uses-permission android:name="android.permission.READ_LOGS" **

uses-permission android:name="android.permission.ACCESS_FINE_LOCATION" ***

uses-permission android:name="android.permission.ACCESS_WIFI_STATE" ****

* To send the report.

** In order to receive the logs above Jelly Bean (api 16).

*** In order to find out, whether the user had internet access or not.

**** In order to find out, whether the user had GPS enabled or not.


# Known issues:
**Was tested only with gmail.
**In case It's not working, You will need to to go to :
https://myaccount.google.com/security?pli=1#connectedapps and "allow less secure apps"

#License

Copyright [2016] [Dgotlieb]

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.


