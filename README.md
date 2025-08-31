[README_RAGNAROK.md](https://github.com/user-attachments/files/22069184/README_RAGNAROK.md)
**************PROYECTO FINAL DE SOFTWARE*************************************

*Ragnarok Barber y tatttoo*

presentado por:

ANDREY OSORIO TABORDA 
DANIELA SANCHEZ VALBUENA

Aplicación web con **frontend** y **backend** separados, diseñada para gestionar usuarios y funcionalidades administrativas.  
Cuenta con autenticación, panel de administración y una interfaz adaptable para su uso en un empresa dedicada al servicio de barbería y tatuajes.

----------------------------**NOTA**----------------------------------------------


**EL SIGUIENTE ES EL LINK DEL PROYECTO DESPLEGADO EN LA NUBE:**

        🖥️   https://ragnarokapp.netlify.app/   

*Importante*

Ver el video del funcionamiento de software primero:

        📽️   https://www.canva.com/design/DAGxqj-kfis/bKfd3Db454E8cKR1I5cBOQ/watch?utm_content=DAGxqj-kfis&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h463cf583f0



---------------------------------------------------------------------

## 🚀 Características principales

- **Autenticación de usuarios** con validación en backend
- **Panel de administración** para gestión de datos
- Interfaz web en HTML, CSS y JavaScript
- API REST desarrollada en Node.js con Express
- Conexión a base de datos MySQL
- Middleware de autenticación para proteger rutas


-----------------------------------------------------------------------
## 📂 Estructura del proyecto

```
PROYECTO_FINAL/
│
├── backend/                                  # Lógica y API del servidor
│ ├── server.js                               # Punto de entrada del servidor
│ ├── db.js                                   # Conexión a la base de datos
│ ├── .env                                    # Variables de entorno
│ ├── package.json                            # Dependencias y scripts de Node.js
│ ├── package-lock.json
│ ├── routes/                                 # Rutas del backend
│ │ ├── admin.js                              # Rutas para administración
│ │ ├── auth.js                               # Rutas de autenticación
│ │ ├── disponibilidad.js                     # Rutas para disponibilidad de artistas
│ │ ├── inventarios.js                        # Rutas de inventarios
│ │ ├── login.js                              # Rutas de login
│ │ ├── logout.js                             # Rutas de logout
│ │ ├── productos.js                          # Rutas de productos
│ │ ├── reservas.js                           # Rutas de reservas
│ │ ├── usuario.js                            # Rutas de usuario individual
│ │ ├── usuarios.js                           # Rutas de gestión de usuarios
│ │ └── ventas.js                             # Rutas de ventas
│ │
│ └── uploads/                                # Archivos subidos
│ └── fotos_usuarios/                         # Imágenes de usuarios
│ ├── *.avif
│ └── *.jpg
│
├── frontend/                                 # Interfaz de usuario
│ ├── css/
│ │ └── estilos.css                           # Estilos principales
│ │
│ ├── img/ # Imágenes generales
│ │
│ ├── imagenes_barberia_slider/               # Imágenes del slider de barbería
│ ├── imagenes_tattoo_slider/                 # Imágenes del slider de tatuajes
│ │
│ ├── scripts/                                # Archivos JavaScript cliente
│ │
│ ├── admin.html                              # Panel de administración
│ ├── barberia.html                           # Página barbería
│ ├── citas.html                              # Página de citas
│ ├── consultaCitas.html                      # Página para consultar citas
│ ├── disponibilidadArtista.html              # Página de disponibilidad del artista
│ ├── index.html                              # Página principal
│ ├── inventario.html                         # Página de inventario
│ ├── login.html                              # Página de inicio de sesión
│ ├── navbar.html                             # Barra de navegación
│ ├── producto.html                           # Página de productos
│ ├── registro.html                           # Página de registro de usuarios
│ ├── reportes.html                           # Página de reportes
│ ├── reservas.html                           # Página de reservas
│ ├── tattoo.html                             # Página tattoo
│ └── usuarios.html                           # Página de usuarios
│
├── .gitignore                                # Archivos/Carpetas ignorados por Git
├── estructura.txt                            # Archivo de referencia de estructura
└── README_RAGNAROK.md                        # Documentación principal del proyecto
```
----------------------------------------------------------------------------------------------------------------


**🛠 Tecnologías utilizadas**

**Backend:**
- Node.js
- Express.js
- MySQL (mysql2 o similar)
- dotenv (variables de entorno)

**Frontend:**
- HTML5
- CSS3
- Boostrap
- JavaScript

**Otros:**
- Git y GitHub para control de versiones
- VS Code / IntelliJ IDEA como entornos recomendados
--------------------------------------------------------------------------------------------------------------------


**📋 Requisitos previos**

Antes de instalar el proyecto, asegúrate de tener instalado:

- Requiere Node.js >= 22 (LTS) puede obtenerse fácilmente desde la página oficial https://nodejs.org/en
- Requiere el gestor de paquetes NPM que también puede ser obtenido desde la página oficial de Node.
- Requiere Base de Datos MariaDB >= 10.2 o MySQL >= 5.7

---------------------------------------------------------------------------------------------------------------------

------------------------**## ⚙️ Instalación y configuración**----------------------------------------------

1. **Clonar el repositorio**

   - ejecutar el comando git clone <https://github.com/AndreyOTCode/Proyecto_Final>
 

2. **Desde la terminal ejecutar estos pasos**
 
        - 1 cd files
        - 2 cd backend (ASEGURATE DE ESTAR EN LA CARPETA BACKEND PARA REALIZAR LOS SIGUIENTES PASOS)
        - 3 npm install

    **Configurar el backend**

        - Crea el archivo .env con el siguiente contenido:

        - DB_HOST=localhost
        - DB_USER=root
        - DB_PASSWORD=tu_password
        - DB_NAME=ragnarok_db

        
    

3. **Iniciar el servidor**
    -  Ejecutar el comando **node server.js**
    -  Al iniciar el servidor se crea automáticamente la base de datos ragnarok_db si no existe.
    -  También se generan tablas iniciales y registros de prueba (**usuarios** y **productos**).


4. **Abrir el frontend**
    - Abre `frontend/index.html` en tu navegador.
    - Cambiar en la url 127.0.0.1  por localhost: (IMPORTANTE PARA UNA OPTIMA INTERACCIÓN)
    - El frontend se comunicará con el backend

------------------------------------- **VIDEOS EXPLICATIVOS DE INSTALACIÓN Y MANUPULACIÓN DEL SOFTWARE**-----------------------------------------------------------------

 *Video de correcta istalación*

                📽️   https://youtu.be/z_U90yme4vM?feature=shared


 *Video de funcionamiento del software local*

                📽️   https://www.youtube.com/watch?v=3VWU1wx4p_0 
                
 ---------------------------------------------------------------------------------------------------------------------------------------



*🧑‍💻 Herramientas recomendadas para versionamiento y desarrollo*

  - Git: Control de versiones

 - GitHub: Repositorio remoto y colaboración

 - Visual Studio Code: Editor ligero con integración Git

- IntelliJ IDEA: IDE con soporte completo para Node.js, Express y Git

---------------------
## 📄 Licencia
Este proyecto es de uso académico. No se permite su uso comercial sin autorización previa.
`
