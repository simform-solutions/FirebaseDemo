# FirebaseDemo
Firebase Cloud Notification

1) Add rules to your root-level build.gradle file, to include the google-services plugin:
```html
buildscript {
    // ...
    dependencies {
        // ...
        classpath 'com.google.gms:google-services:3.0.0'
    }
}
```

2) Add the FCM dependency to your app-level build.gradle file:

```html
dependencies {
     compile 'com.google.firebase:firebase-messaging:9.2.1'
}
```

3) Add this 2 service in your meanfieast.xml
```html
<service
    android:name=".MyFirebaseMessagingService">
    <intent-filter>
        <action android:name="com.google.firebase.MESSAGING_EVENT"/>
    </intent-filter>
</service>
 

...

  <service
    android:name=".MyFirebaseInstanceIDService">
    <intent-filter>
        <action android:name="com.google.firebase.INSTANCE_ID_EVENT"/>
    </intent-filter>
</service>
 ```

 
