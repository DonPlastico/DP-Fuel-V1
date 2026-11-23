# ⛽ DP-Fuel V1

**DP-Fuel V1** es un sistema ligero, moderno y optimizado de gestión de combustible para servidores de **FiveM**. Combina una arquitectura modular en Lua con una interfaz NUI reactiva desarrollada en **React, TypeScript y Vite**, ofreciendo un rendimiento fluido y una experiencia limpia para los jugadores.

<h1>Fotos</h1>

![image](https://github.com/user-attachments/assets/5f39dc98-d8b3-49c0-be09-71a7e008522e)
![image](https://github.com/user-attachments/assets/df1cb4ea-90dd-4702-b7f6-ab839b4b0a18)

<h2>Configuración facil de entender</h2>

![image](https://github.com/user-attachments/assets/e89feec3-b0e5-4981-97c2-c1c4e3270050)
![image](https://github.com/user-attachments/assets/0dc4a9f1-9f68-41cf-829e-5e4722a42226)

## ✨ Características Principales

* **⚡ Interfaz NUI Moderna y Fluida:** Construida con React, TypeScript y Vite (`web/`), garantizando tiempos de carga instantáneos y bajo consumo de recursos.
* **🧩 Arquitectura Modular:** Código separado en módulos limpios tanto en cliente (`client/Modules/`) como en servidor (`server/Modules/`) para facilitar su lectura y mantenimiento.
* **⚙️ Configuración Sencilla:** Archivo `config.lua` claro y directo para ajustar precios, consumo, gasolineras y comportamiento del sistema en pocos minutos.
* **🪶 Ligero y Optimizado:** Diseñado para mantener el consumo de `resmon` al mínimo en todo momento.

## 📂 Estructura del Proyecto

```text
DP-Fuel-V1/
├── client/
│   ├── Modules/
│   │   └── Functions.lua       # Funciones auxiliares del lado cliente
│   └── client.lua              # Lógica principal de combustible y repostaje
├── server/
│   ├── Modules/
│   │   └── Functions.lua       # Funciones auxiliares del lado servidor
│   └── server.lua              # Validaciones y gestión económica en servidor
├── web/
│   ├── build/                  # Interfaz NUI compilada lista para producción
│   ├── src/                    # Código fuente de la UI (React + TypeScript)
│   │   ├── components/         # Componentes visuales (App.tsx)
│   │   ├── hooks/              # Hooks personalizados (useNuiEvent.ts)
│   │   ├── providers/          # Gestión de visibilidad NUI
│   │   └── utils/              # Utilidades y comunicación fetchNui
│   ├── package.json            # Dependencias del proyecto web
│   └── vite.config.ts          # Configuración de empaquetado Vite
├── config.lua                  # Configuración principal del recurso
├── fxmanifest.lua              # Manifiesto del recurso FiveM
└── LICENSE                     # Licencia del proyecto
```

## 🚀 Instalación

1. **Descarga** el repositorio y extrae el contenido.
2. Copia la carpeta `DP-Fuel v1` (recomendado renombrarla sin espacios, por ejemplo `DP-Fuel-V1`) dentro de la carpeta `resources` de tu servidor de FiveM.
3. Añade el recurso a tu archivo `server.cfg`:
   ```cfg
   ensure DP-Fuel-V1
   ```
4. Revisa y ajusta los parámetros en `config.lua` según las necesidades de tu servidor.
5. Reinicia tu servidor o ejecuta `refresh` y `ensure DP-Fuel-V1` en la consola.

## 🛠️ Desarrollo de la Interfaz (Opcional)

El recurso ya incluye la carpeta `web/build/` compilada y lista para usar. Si deseas modificar el diseño de la interfaz en `web/src/`:

1. Abre una terminal dentro de la carpeta `web/`.
2. Instala las dependencias:
   ```bash
   npm install
   ```
3. Compila los cambios para FiveM:
   ```bash
   npm run build
   ```

## 📄 Licencia

Este proyecto se distribuye bajo los términos incluidos en el archivo `LICENSE` del repositorio.
