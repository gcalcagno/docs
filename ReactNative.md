# COMANDOS NECESARIOS

##

### LUEGO DE CAMBIOS EN ANDROID
$ curl "http://localhost:8081/index.android.bundle?platform=android" -o "android/app/src/main/assets/index.android.bundle"

##

### CLEAN GRADLE
cd android/ && ./gradlew clean
cd .. && react-native run-android

##

### LOG ANDROID
react-native log-android

### RUN ANDROID
react-native run-android
