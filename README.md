# MyMusic! 🎵

**MyMusic!** es una aplicación móvil de reproducción musical desarrollada en la plataforma **MIT App Inventor**. Este repositorio funciona exclusivamente como el servidor para almacenar y servir los archivos de audio (`.mp3`) y las portadas de los álbumes (`.jpg`) de forma rápida y directa.

La lógica del sistema funciona bajo una arquitectura desacoplada:
1. **Base de Datos:** Un documento de **Google Sheets** almacena los datos de las canciones (Título, Artista, Categoría, Portada y Archivo .mp3).
2. **Servidor de Descarga:** **MIT App Inventor** consulta la base de datos y los descarga desde este repositorio de **GitHub** para su reproducción local.

---

## 📂 Estructura del Repositorio

Los recursos multimedia se encuentran organizados de manera simétrica por su categoría musical, asegurando rutas limpias y predecibles:

```text
MyMusic/
├── README.md               # Documentación del repositorio
├── audio/                  # Archivos de sonido de las canciones
│   ├── pop/
│   │   └── ...
│   └── rock/
│       └── ...
│   
└── portadas/               # Imágenes de carátulas de los temas
    ├── pop/
    │   └── ...
    └── rock/
        └── ...
