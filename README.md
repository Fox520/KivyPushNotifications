# KivyPushNotifications
Repository for https://www.youtube.com/watch?v=006LU_XeQwM

(**DEPRECATED in favour of this** https://github.com/Fox520/pushyy)
-------

## Here's a simpler approach
1. Run `git clone https://github.com/Fox520/python-for-android` or manually download it

2. Replace pythonforandroid/bootstraps/common/build/google-services.json with your [own](https://support.google.com/firebase/answer/7015592)
3. Open buildozer.spec file
- Set `p4a.source_dir` to the full path of the folder cloned in step 1.

- Set `android.gradle_dependencies` to `com.google.firebase:firebase-messaging,com.google.firebase:firebase-analytics`

* Set `android.add_src` to `MyFirebaseMessagingService.java`

4. Place `MyFirebaseMessagingService.java` from this repository to your project folder (the one with `main.py`)
