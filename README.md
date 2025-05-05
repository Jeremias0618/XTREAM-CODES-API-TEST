# 📺 [XTREAM CODES API TEST](https://github.com/Jeremias0618)

Aplicación web diseñada para interactuar directamente con servidores **Xtream Codes / XUI One**, permitiendo al usuario visualizar y reproducir contenido de **TV en vivo**, **Series**, **Películas (VOD)** y realizar búsquedas multimedia a través de la **API de TMDB**.

> Esta herramienta está pensada como una interfaz de prueba y exploración para desarrolladores o administradores de paneles IPTV Xtream Codes, con una estructura de proyecto modular, mantenible y optimizada.

---

## 🔧 Características principales

✅ Compatible con la API oficial de Xtream Codes (usando `player_api.php`)  
✅ Autenticación mediante IP/Dominio, Usuario y Clave  
✅ Guardado temporal de credenciales (caché local de 10 minutos)  
✅ Navegación paginada y búsqueda dinámica por nombre  
✅ Reproductor personalizado:
- 🎦 **JW Player** para `.mp4`
- 🎞️ Reproductor nativo para `.m3u8`, `.mkv`, `.webm` 

✅ Visualización adaptada a dispositivos móviles  
✅ Buscador TMDB con visualización enriquecida: portada, sinopsis, reparto, tráiler y más  
✅ Código organizado profesionalmente en carpetas: `html/`, `css/`, `js/`, `images/`, `libs/`

---

## 🗂️ Estructura del proyecto

```

XTREAM-CODES-API-TEST/
│
├── index.html                 # Página de inicio (enlace a las demás secciones)
├── live_tv.html               # Reproductor de canales en vivo
├── series.html                # Navegación y reproducción de series IPTV
├── vod.html                   # Películas bajo demanda
├── tmdb_api.html              # Buscador de contenido vía TMDB
│
├── css/                       # Estilos separados por sección
│   ├── live_tv.css
│   ├── series.css
│   ├── vod.css
│   └── tmdb.css
│
├── js/                        # Scripts separados por sección
│   ├── live_tv.js
│   ├── series.js
│   ├── vod.js
│   └── tmdb.js
│
├── images/                    # Recursos gráficos
│   ├── logo.png
│   └── icon.png
│
└── libs/                      # Bibliotecas externas si se desean incluir offline
└── jwplayer.js

```

---

## 🧪 Requisitos técnicos

- Navegador moderno compatible con ES6 (Chrome, Firefox, Edge)
- Conexión activa a un servidor Xtream Codes/XUI One
- API Key válida de [TMDB](https://www.themoviedb.org/) (para `tmdb_api.html`)
- Conexión HTTPS preferida para evitar problemas con contenido mixto (Opcional)

---

## 🚀 ¿Cómo usar?

1. Clona o descarga el repositorio.
2. Abre cualquier archivo `.html` directamente desde tu navegador.
3. Introduce tus credenciales Xtream Codes:
   - IP/Dominio
   - Usuario
   - Contraseña
4. Pulsa **"Cargar"** y navega por los contenidos.

> El sistema recuerda tus datos por 10 minutos usando almacenamiento local (localStorage).

---

## 📦 Detalles por sección

### 🔴 `live_tv.html`
- Carga todos los canales IPTV del usuario.
- Muestra 40 canales por página con miniaturas y nombres.
- Al hacer clic se abre un modal con el canal en vivo.
- Usa JW Player para `.m3u8`.

### 📚 `series.html`
- Muestra una grilla de 5x8 con portadas de series.
- Clic en una serie muestra los capítulos disponibles.
- Elige un capítulo y se reproduce con el reproductor correspondiente.

### 🎥 `vod.html`
- Carga todas las películas disponibles en el servidor IPTV.
- Reproducción con JW Player para `.mp4` y nativo para otros.

### 🔍 `tmdb_api.html`
- Permite ingresar una API key de TMDB.
- Busca por título películas, series o animes.
- Muestra sinopsis, géneros, año, reparto, fondo, portada y tráiler.

---

## 🔐 Seguridad y privacidad

- Ningún dato se transmite a terceros.
- Las credenciales solo se almacenan localmente en tu navegador durante 10 minutos.
- Si deseas mayor seguridad, puedes desactivar el almacenamiento temporal modificando el código JavaScript.

---

## ⚙️ Personalización

- Puedes reemplazar `JW Player` por cualquier otro reproductor si cuentas con una licencia propia.
- Puedes modificar los estilos en la carpeta `css/` o usar frameworks como Tailwind, Bootstrap, etc.
- Para producción, se recomienda minificar CSS y JS.

---

## 📄 Licencia

Este proyecto se distribuye bajo la licencia MIT.  
Eres libre de usar, modificar y distribuir este software bajo los términos de dicha licencia.


---


## 🤝 Créditos y agradecimientos

- [JW Player](https://www.jwplayer.com/)
- [TMDB API](https://developers.themoviedb.org/)
- [Xtream Codes API](https://github.com)
- Iconos libres de [Flaticon](https://www.flaticon.com/) 


---


## 📬 Contacto

Desarrollado por **[Yeremi T](https://github.com/Jeremias0618)**  
📧 ¿Tienes dudas o sugerencias? Puedes enviar un mensaje directo.


---


## 📢 Descargo de responsabilidad

Este proyecto ha sido desarrollado únicamente con fines educativos y de prueba.

- **No promueve, apoya ni distribuye contenido protegido por derechos de autor.**
- **No incluye ningún tipo de contenido ilegal, enlaces m3u/m3u8, listas IPTV, VOD ni credenciales.**
- El uso de este sistema con servidores Xtream Codes de terceros o sin autorización puede infringir leyes locales sobre propiedad intelectual o acceso a servicios privados.
- El desarrollador **no se hace responsable** por el uso indebido del código aquí publicado.
- Es responsabilidad del usuario cumplir con las leyes de su país y respetar los términos de servicio de cualquier proveedor.

Este repositorio **no tiene relación con Xtream Codes, TMDB ni JW Player**, sus marcas, software o servicios.


