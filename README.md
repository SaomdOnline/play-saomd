# play-saomd
`Sword Art Online: Memory Defrag` App Launcher

## Instructions
For this to work, you will need to add the following to `AndroidManifest.xml`
```xml
<data android:scheme="defrag-native" android:host="launch" />
```

Add this line here and recompile APK:
```xml
<intent-filter>
    <action android:name="android.intent.action.VIEW"/>
    <category android:name="android.intent.category.DEFAULT"/>
    <category android:name="android.intent.category.BROWSABLE"/>
    <data android:scheme="saomemorydefrag"/>
    <data android:scheme="defrag-native" android:host="launch" />
</intent-filter>
```
