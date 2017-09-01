# ANDROID

### RUN ANDROID
react-native run-android

### LUEGO DE CAMBIOS EN ANDROID
$ curl "http://localhost:8081/index.android.bundle?platform=android" -o "android/app/src/main/assets/index.android.bundle"

### CLEAN GRADLE
cd android/ && ./gradlew clean
cd .. && react-native run-android

### LOG ANDROID
react-native log-android


##
##

# IOS

### RUN IOS
react-native run-ios

### LOG ANDROID
react-native log-ios
