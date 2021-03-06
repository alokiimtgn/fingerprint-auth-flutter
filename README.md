# flutter_fingerprint_auth

Fingerprint Authentication in Flutter

## Introduction

Prerequisite: fingerprint sensor in mobile device you are testing on.

## Steps

1. Create new flutter project. I have created a new project named as “flutter_fingerprint_auth”

2. Add a dependency for plugin “local_auth” in file “pubspec.yaml” in project root directory

```
dependencies:
 flutter:
   sdk: flutter
 cupertino_icons: ^0.1.2
 local_auth: ^0.4.0+1
```
NOTE: I have tried local_auth version 0.5.2+3 but it is not working but version 0.4.0+1 working for me.
	And run flutter packages get

3. Add a permission for android in android/app/src/main/AndroidManifest.xml
```
<manifest xmlns:android="http://schemas.android.com/apk/res/android"
          package="com.example.app">
  <uses-permission android:name="android.permission.USE_FINGERPRINT"/>
<manifest>
```

 
## MAY BE ERRORS:
    Error: import androidx.annotation.NonNull;
    Solution : 
    Put android.useAndroidX=true
    android.enableJetifier=true
    In android/gradle.properties file
 
 