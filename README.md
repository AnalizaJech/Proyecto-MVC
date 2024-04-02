### Estructura de directorios sugerida para un proyecto MVC:

<pre>
project/
│
├── app/
│   ├── Controllers/
│   │   └── HomeController.php
│   │   └── UserController.php
│   │   └── ...
│   │
│   ├── Models/
│   │   └── UserModel.php
│   │   └── ...
│   │
│   ├── Views/
│   │   └── home.php
│   │   └── user.php
│   │   └── ...
│   │
│   ├── Routes/
│   │   └── web.php
│   │   └── api.php
│   │   └── ...
│   │
│   └── Helpers/
│
├── public/
│   ├── css/
│   │   └── style.css
│   │   └── ...
│   │
│   ├── js/
│   │   └── script.js
│   │   └── ...
│   │
│   ├── img/
│   │   └── logo.png
│   │   └── ...
│   │
│   └── index.php
│
└── config/
    └── database.php
    └── ...
</pre>

> [!NOTE]
> En esta estructura, los controladores, modelos y vistas están separados en directorios correspondientes dentro de la carpeta app/. 
El enrutamiento se define en archivos específicos dentro del directorio Routes/. 
Los archivos estáticos (CSS, JavaScript, imágenes) se almacenan en la carpeta public/, y el archivo principal de entrada (index.php) se encuentra en este directorio también. 
Los archivos de configuración, como la configuración de la base de datos, pueden estar en el directorio config/.

#
## Estructura típica para un proyecto web utilizando el patrón de diseño MVC (Modelo-Vista-Controlador)

<pre>
proyecto/
├── app/
│   ├── controllers/
│   │   ├── HomeController.php
│   │   └── ...
│   ├── models/
│   │   ├── User.php
│   │   └── ...
│   └── views/
│       ├── home/
│       │   ├── index.php
│       │   └── ...
│       ├── layouts/
│       │   ├── header.php
│       │   ├── footer.php
│       │   └── ...
│       └── ...
├── config/
│   ├── config.php
│   └── database.php
├── public/
│   ├── assets/
│   │   ├── css/
│   │   │   ├── styles.css
│   │   │   └── ...
│   │   ├── js/
│   │   │   ├── scripts.js
│   │   │   └── ...
│   │   └── images/
│   │       ├── logo.png
│   │       └── ...
│   ├── index.php
│   └── .htaccess
├── vendor/
│   ├── composer/
│   └── ...
├── .gitignore
├── composer.json
└── README.md
</pre>


Te explico qué va dentro de cada carpeta y archivo:

- app/: Contiene los archivos principales de la aplicación.
- controllers/: Contiene los archivos de los controladores (por ejemplo, HomeController.php).
- models/: Contiene los archivos de los modelos (por ejemplo, User.php).
- views/: Contiene los archivos de las vistas (por ejemplo, index.php dentro de home/).
- layouts/: Contiene los archivos de plantillas reutilizables (por ejemplo, header.php y footer.php).
- config/: Contiene archivos de configuración.
- config.php: Archivo de configuración general de la aplicación.
- database.php: Archivo de configuración de la conexión a la base de datos.
- public/: Contiene los archivos públicos accesibles desde el navegador.
- assets/: Contiene los archivos estáticos (CSS, JavaScript, imágenes, etc.).
- css/: Contiene los archivos CSS (por ejemplo, styles.css).
- js/: Contiene los archivos JavaScript (por ejemplo, scripts.js).
- images/: Contiene las imágenes (por ejemplo, logo.png).
- index.php: Archivo de entrada principal de la aplicación.
- .htaccess: Archivo de configuración del servidor web (por ejemplo, para enrutamiento amigable con URLs).
- vendor/: Contiene las librerías y dependencias instaladas mediante Composer (manejador de paquetes de PHP).
- .gitignore: Archivo que indica qué archivos/carpetas deben ser ignorados por el sistema de control de versiones Git.
- composer.json: Archivo de configuración de Composer, que lista las dependencias del proyecto.
- README.md: Archivo de documentación del proyecto.

Dentro de los archivos PHP, podrías encontrar código como:

- controllers/HomeController.php: Contiene la lógica de control para renderizar la página de inicio.
- models/User.php: Contiene la lógica para interactuar con la tabla de usuarios en la base de datos.
- views/home/index.php: Contiene el código HTML y PHP para mostrar la página de inicio.

En los archivos JavaScript, podrías encontrar código Ajax y jQuery para realizar solicitudes asíncronas al servidor y manipular el DOM.

La estructura básica puede variar según los requerimientos y prácticas de tu proyecto.


