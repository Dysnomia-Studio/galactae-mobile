# galactae-mobile

# How to build:

- Put release.keystore next to this file
- Set "storePassword" and "password" fields to the one stored on Keepass
- npm i
- npm run prepare
- `JAVA_HOME="C:\Program Files\Microsoft\jdk-22" npm run build:release`

# Change Android version number:

- (May be needed:) Update android SDK
- Open config.xml
- Edit `<preference name="android-minSdkVersion" value="VERSION" />`

# Update android SDK

- Run Git bash as an administrator
- `cd "/c/Program Files (x86)/Android/android-sdk/cmdline-tools/12.0/bin"` 
- `JAVA_HOME="C:\Program Files\Microsoft\jdk-22" ./sdkmanager.bat "platforms;android-VERSION"` 
- `JAVA_HOME="C:\Program Files\Microsoft\jdk-22" ./sdkmanager.bat --update` 

# Change app version number

- `npm version patch` (to edit package.json / package-lock.json)
- Edit version field in root element in config.xml