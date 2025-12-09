# Doby el Goloso — Cordova Project

Esta carpeta contiene el juego HTML listo para empaquetar como APK usando Apache Cordova.

## Qué hay aquí
- `www/index.html` — el juego HTML/CSS/JS (prototipo).
- `config.xml` — configuración Cordova básica.
- `package.json` — script útil para construir.

## Opciones para obtener el APK

### 1) Construir localmente (sin Android Studio GUI, pero necesitas SDK)
Instala:
- Node.js
- Java JDK
- Android SDK / Command-line tools

Comandos:
```bash
npm install -g cordova
npm install
cordova platform add android
cordova build android
```
El `.apk` estará en `platforms/android/app/build/outputs/apk/debug/`

### 2) Usar un build service ONLINE (no necesitas Android Studio ni instalar SDK)
Servicios recomendados: Ionic Appflow, Codemagic, Appcircle.
Estos servicios pueden tomar tu repositorio (GitHub/ZIP) y generar el APK en la nube. Puedes descargar el `.apk` cuando termine la compilación.

Referencias:
- Ionic Appflow: https://ionic.io/appflow
- Codemagic: https://codemagic.io
- Appcircle: https://appcircle.io

## Notas
- No puedo compilar el APK directamente desde este entorno, pero este proyecto está preparado para que lo compiles localmente o lo subas a un servicio online.
- Si quieres que lo suba todo a un repositorio GitHub con instrucciones paso a paso para Codemagic/Appflow, lo puedo generar aquí mismo.

