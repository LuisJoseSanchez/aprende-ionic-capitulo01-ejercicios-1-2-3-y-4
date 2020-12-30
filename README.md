# Soluciones a los ejercicios 1, 2, 3 y 4 del capítulo 1

## Ejercicio 1

### Creación de un proyecto en Ionic Versión 1 (con AngularJS)

Antes de nada, hay que instalar Python 2 en caso de no tenerlo instalado en el sistema, aunque tengamos instalada una versión más reciente como por ejemplo Python 3.

```console
sudo apt install python2
```

Creamos un proyecto en blanco:

```console
ionic start exercise01a blank --type=ionic1
```

La creación del proyecto podría provocar errores relativos al CSS. En tal caso, habría que instalar `node-sass`, borrar el directorio `node_modules` y actualizar las dependencias: 

```console
cd exercise01a
npm install node-sass
rm -Rf node_modules
npm install
```

No sería de extrañar que se siguieran produciendo errores. Ionic 1 ya es muy antiguo y hace uso de librerías obsoletas. Esto no va a afectar en ningún modo a los proyectos que realicemos con versiones modernas de este framework. 

Si el proyecto se ha creado correctamente, se puede lanzar el servidor:

```console
ionic serve
```

<img src="ionic1blank.png">

Estructura de directorios y ficheros:

```console
exercise01a
├── bower.json
├── gulpfile.js
├── hooks
│   ├── after_prepare
│   └── README.md
├── ionic.config.json
├── ionic.starter.json
├── node_modules
│   │
.   .
.   .
.   .
├── package.json
├── package-lock.json
├── scss
│   └── ionic.app.scss
└── www
    ├── css
    ├── img
    ├── index.html
    ├── js
    ├── lib
    ├── manifest.json
    └── service-worker.js
```

Como se puede observar, en un proyecto de la versión 1 de Ionic, el grueso de la aplicación está en la carpeta `www`. Dentro de ese directorio está `index.html` que hace las veces de plantilla HTML.

La lógica de negocio estaría contenida dentro de la carpeta `js`, los estilos en la carpeta `css` y las imágenes en `img`.

Se trata de una estructura muy simple, parecida a lo que sería un proyecto de HTML con Javascript sin ningún framework.

**En Ionic 1 se utiliza AngularJS** (versión 1.X). Cuando se liberó esta versión de Ionic, todavía no existía **Angular** a secas (versión 2+), por tanto, la lógica de negocio se programaba directamente en Javascript.

### Creación de un proyecto en Ionic Versión 3 (con Angular)

Creación del proyecto:

```console
ionic start exercise01b blank --type=ionic-angular
```

<img src="ionic3blank.png">

Estructura de directorios y ficheros:

```console
exercise01b
├── ionic.config.json
├── node_modules
.   .
.   .
.   .
├── package.json
├── package-lock.json
├── src
│   ├── app
│   ├── assets
│   ├── index.html
│   ├── manifest.json
│   ├── pages
│   ├── service-worker.js
│   └── theme
├── tsconfig.json
├── tslint.json
└── www
    ├── assets
    ├── build
    ├── index.html
    ├── manifest.json
    └── service-worker.js
```

Como podemos comprobar, hay más diferencias que similitudes en la estructura de directorios de un proyecto de la versión 2/3 con respecto a otro de la versión 1.

En esta versión, el código fuente de la aplicación está en la carpeta `src` mientras que en la carpeta `www` se colocará el código de la aplicación una vez compilada, lista para su despliegue.

Si indagamos un poco dentro del directorio `app` o en `pages` (donde se encuentra la página principal que viene por defecto) encontraremos archivos con la extensión `.ts`. Estos archivos contienen código en **Typescript**, lo que nos da una pista que nos indica que estamos ya ante un proyecto en el que se usa **Angular** y no **AngularJS**.

### Creación de un proyecto en Ionic Versión 4 o posterior (con Angular)

```console

```

Estructura de directorios y ficheros:

```console

```

## Ejercicio 2

```console

```

## Ejercicio 3

```console

```

## Ejercicio 4

```console

```
