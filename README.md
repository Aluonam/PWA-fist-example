# PWA-fist-example

## Aplicación Web Progresiva

Permite a la app web ofrecer servicios de instalación en un dispositivo como si se tratase de una app móvil.
**Pasos:**

1. Crear proyecto con react-next de forma normal:
Con react Router App

2. Entrar en web de configuración de PWA: rellena los datos y descarga el zip.
*Inserta una imagen en formato PNG para que sea el logo de tu app.
Copia los datos del zip y pégalos en tu proyecto en la carpeta public.
Cambia el nombre del archivo manifest a manifest.json
*En caso de que no hayas instalado la app de React con Router. El archivo que tienes que modificar es: pages -> document.js

3. Dentro de tu proyecto -> app -> layout.js  modifica el export const metadata 
// Incluye manifest. icons y themeColor
export const metadata = {
  title: 'Create Next App',
  description: 'Generated by create next app',
    // Aquí incluimos los datos de manifest:
  manifest: "/manifest.json",
  icons: {
  apple: "/icon.png"
  },
  themeColor: "#000000"
}
4. Tumba y levanta el proyecto y abre el localhost.
5. En el localhost aparecerá un icono que te permite descargar tu app como si fuese móvil. 
