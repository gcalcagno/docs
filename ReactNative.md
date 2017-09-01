# ANDROID

### RUN ANDROID
```
$ react-native run-android
```
### LUEGO DE CAMBIOS EN ANDROID
```
$ curl "http://localhost:8081/index.android.bundle?platform=android" -o "android/app/src/main/assets/index.android.bundle"
```
### CLEAN GRADLE
```
$ cd android/ && ./gradlew clean
$ cd .. && react-native run-android
```
### LOG ANDROID
```
$ react-native log-android
```

### EXPORTAR PROYECTO
el .apk se guarda en /android/app/build/outputs/app-release.apk
```
$ cd android && ./gradlew assembleRelease
$ cd android && ./gradlew assembleDebug

```

##
##

# IOS

### RUN IOS
```
$ react-native run-ios
```

### LOG ANDROID
```
$ react-native log-ios
```

### EXPORTAR PROYECTO
```
Edit Scheme
- Run (debug)
- Archive (Release)

PASAR AL IPHONE
run -> release
conectar Iphone
Seleccionar IPHONE
Play con el celular conectado
```
