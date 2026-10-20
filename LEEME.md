# Veritup Demo → APK

Maqueta de Veritup lista para convertirse en app Android. Es una versión de prueba: los pagos se simulan, los montos son ficticios y los datos quedan solo en el teléfono.

## Generar el APK (sin instalar nada en tu compu)

1. Creá una cuenta gratis en github.com y un repositorio nuevo (por ejemplo `veritup-demo`).
2. Subí todo el contenido de esta carpeta, incluida la carpeta oculta `.github`.
   Lo más fácil: en el repositorio tocá **Add file → Upload files** y arrastrá los archivos y carpetas.
   Si la carpeta `.github` no aparece (en Mac y Windows suele estar oculta), creala a mano: **Add file → Create new file**, escribí como nombre `.github/workflows/build-apk.yml` y pegá el contenido de ese archivo.
3. Entrá a la pestaña **Actions**. La compilación arranca sola y tarda unos 5 minutos.
4. Cuando termina, el APK queda publicado en **Releases** con este link fijo:

   `https://github.com/Alanrtobal01/Veritup-Apk/releases/download/demo/veritup-demo.apk`

Cada vez que cambies `www/index.html`, el APK se vuelve a generar y el link sigue siendo el mismo.

## Poner la descarga en la web

El botón **Descargar .apk** de la pantalla de descarga ya apunta a ese link.

## Instalarlo en un Android

Al abrir el APK, Android pide permitir la instalación desde esa fuente. Es normal en apps que no vienen de Google Play.

## Archivos

- `www/index.html`: la maqueta.
- `capacitor.config.json`: nombre de la app (`Veritup Demo`) e identificador.
- `.github/workflows/build-apk.yml`: la receta que compila el APK.
