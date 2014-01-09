AndroidArgon
============

#### What is AndroidArgon and what's new?

This is a proof of concept of Argon for Android. Thanks to an updated WebView in Android 4.4 SDK [1] it is now possible to have an app with a camera in the background view and with WebView in the foreground that contains complex CSS3D objects. Webview supports transparency as seen on screenshots below. 

As an example I developed an app that is integrated with a ImageTargets provided with vuforia [2]. After launching the app:

1. In the first WebView there's a sample webpage that contains multiple DIV elements rotated by different angles in 3D. In the background there's a camera. When camera is above sample image provided by vuforia, a teapot is rendered. See a screenshot in Preview Section. There is no problem with performance of the app even if there's a large amount of these DIV. 
2. To see a second example, click on a button "Go to CSS3D Periodic Table". In the background you can still see a camera and teapot, in the foreground there's a periodic table in CSS 3D [3]. See screenshot 2.
Once again there are no performance issues and website is very responsive. 


#### Preview

**Screenshot 1** - camera in the background with teapot, and webview with a sample webpage with transparent background in the foregorund:
![Alt text](https://raw2.github.com/pkwiecien/AndroidArgon/master/screenshots/device-2014-01-09-113733.png "Screenshot 1 - camera in the background with teapot, and webview with a sample webpage with transparent background in the foregorund")

**Screenshot 2** - camera in the background with teapot, and webview with a sample webpage in the foreground:
![Alt text](https://raw.github.com/pkwiecien/AndroidArgon/master/screenshots/device-2013-12-09-122533.jpg "Screenshot 2 - camera in the background with teapot, and webview with a sample webpage in the foreground")

**Screenshot 3** - camera in the background with teapot, and webview with Periodic Table in the foreground:
![Alt text](https://raw.github.com/pkwiecien/AndroidArgon/master/screenshots/device-2013-12-09-122623.jpg "Screenshot 3 - camera in the background with teapot, and webview with Periodic Table in the foreground")

#### How to run the app?
* Pull repository
* Open ADT (or eclipse with ADT), install Android 4.4 SDK and vuforia if needed (see requirements below)
* Import AndroidArgon as exisiting Android project into ADT
* Add QCAR_SDK_ROOT into Java Build Path, see: Section "Set the QCAR environment variable" 
in https://developer.vuforia.com/resources/dev-guide/step-2-installing-vuforia-sdk
* Run project as Android application
* 
#### Requirements:
* Android 4.4 SDK (API 19) installed
* vuforia installed, follow: https://developer.vuforia.com/resources/sdk/android

#### Test environment:
* ADT for Mac
* Nexus 7 Tablet (second generation) with Android 4.4 

#### References

* [1] https://developer.android.com/guide/webapps/migrating.html
* [2] https://developer.vuforia.com/resources/sample-apps/image-targets-sample-app
* [3] http://threejs.org/examples/css3d_periodictable.html
