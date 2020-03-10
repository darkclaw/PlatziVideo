# REACT Server Side Rendering 

_Esta arquitectura es una propuesta inicial, para comenzar cualquier desarrollo Frontend en KEA Digital. Con Tecnología JavaScript, NodeJs, REACT, REDUX, Webpack, Express (SSR), MongoDB y SASS._

## Comenzando 

_Estas instrucciones te permitirán obtener una copia del proyecto en funcionamiento en tu máquina local para propósitos de desarrollo y pruebas._

Mira **Deployment** para conocer como desplegar el proyecto en producción y desarrollo.


### Pre-requisitos 📋

_Es necesario instalar npm, para eso necesitamos instalar node en nuestro ambiente local, las siguientes instrucciones son para MacOS (la versión que se tiene al momento de realizar este documento es 10.14.6)_

```
brew update

brew install node

brew upgrade node
```

_Antes de instalar las dependencias es necesario definir en que ambiente trabajaremos nuestro proyecto, para eso creamos el archivo .env, si ya se encuentra en el proyecto lo modificamos._

_El archivo .env debe conter los siquientes parametros_

_.env development_
```
ENV=development
PORT=3000
```

_.env production_
```
ENV=production
PORT=8080
```

### Instalación 🔧

_Los siguientes comandos son para actualizar e instalar las dependencias dependiendo del ambiente, las opcines que tenemos son development y production. Algunas dependencias solo se usan en production y otras en development como veremos más adelante_

_Comencemos actualizando las dependencias del package.json con los siguientes comandos_

```
#verify dependency out date
npm outdated

#update dependencies
npm update
```

_Ahora comencemos la instalción de las dependecias, las sigientes dependencias son para production y development_

```
#install dependency babel 
npm install @babel/register

#install dependency nodemon restar server 
npm install nodemon --dev

#install dotenv enviroment 
npm install dotenv

#install dependency webpack 
npm install webpack-dev-middleware webpack-hot-middleware --dev

npm install webpack

#npm install dependency history and react-router-config
npm install history react-router-config

#npm install dependency react-router
npm install react-router 

#npm install dependency ignore-styles
npm install ignore-styles 

#npm install dependency eslint-loader. 
# A ESlint loader for webpack Note: You also need to install eslint from npm, if you haven't already: npm install eslint --save-dev

npm install eslint-loader --save-dev

#npm install dependency eslint
npm install eslint --save-dev

```

_Las siguientes dependencias son para el ambiente development_

```
#npm install dependency react-hot-loader. Mode HotModuleReplacementPlugin. env development 
npm install react-hot-loader --dev

#npm install dependency asset-require-hook. env development 
npm install asset-require-hook

```

_Las siguientes dependencias son para el ambiente production_

```
#npm install dependency helmet  env production
#https://helmetjs.github.io/ Helmet helps you secure your Express apps by setting various HTTP headers. It’s not a silver bullet, but it can help!
npm install helmet

#npm install dependency compression-webpack-plugin. env production 
npm install compression-webpack-plugin --save-dev

#npm install dependency compression-webpack-plugin. 
#This plugin uses terser to minify your JavaScript. env production 

npm install terser-webpack-plugin --save-dev

#npm install dependency optimize-css-assets-webpack-plugin. env production
#Note: For webpack v3 or below please use optimize-css-assets-webpack-plugin@3.2.0. The optimize-css-assets-webpack-plugin@4.0.0 version and above supports webpack v4

npm install --save-dev optimize-css-assets-webpack-plugin@4.0.0

#npm install dependency npm install webpack-manifest-plugin. env production 
npm install webpack-manifest-plugin

```


## Despliegue 📦

_Después de instalar las dependencias dependiendo del ambiente, podemos hacer el despliegue de nuestro proyecto para verlo en el navegador_

_Para el ambiente de desarrollo (env development), estan los siguientes comandos_

_Si queremos visualizar el proyecto en mode development, ejecutamos la siguiente instrucción_
```
npm run start
```

_Si queremos ejecutar el proyeco en modo Hot Module Replacement, esta funcionaldad permite hacer el despligue pero si hacemos una modificación al código lo mostrara enseguida sin necesidad de recargar el proyecto o reconstruir. Para esta opción, ejecutamos el siguiente comando_

```
npm run start:dev
```

_Antes de realizar el despligue en producción es recomendable usar ESLint. ESLint es una herramienta de análisis de código estático para identificar patrones problemáticos encontrados en el código JavaScript. Ejecutamos la siguinete instrucción oara analizar nuestro código_

```
npm run lint
```

_El despliegue en producción de realiza ejecutando las siguientes instrucciones_

_Antes de iniciar el servidor es necesario construir los archivos, para esto ejecutamos el siguiente comando_

```
npm run build
```

_Después de construir el proyecto para producción, se ejecuta el siguiente comando para iniciar el servidor en el puerto indicado en el archivo .env_

```
node src/server
```

## Construido con 🛠️

_Menciona las herramientas que utilizaste para crear tu proyecto_

* [REACT](https://reactjs.org/) - REACT  A JavaScript library for building user interfaces.
* [Git](https://git-scm.com/) - Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.
* [REDUX](https://redux.js.org/) - A Predictable State Container for JS Apps.
* [webpack](https://webpack.js.org/) - webpack is a static module bundler for modern JavaScript applications.
* [Node.js](https://nodejs.org/) - Node.js® is a JavaScript runtime built on Chrome's V8 JavaScript engine.
* [mongoDB](https://www.mongodb.com/) - MongoDB is a general purpose, document-based, distributed database built for modern application developers and for the cloud era.
* [JavaScript](https://js.org/) - JavaScript.
* [ESLint](https://eslint.org/) - Find and fix problems in your JavaScript code.


## Autores ✒️

_Involucrados en el proyecto_

* **Iván de Jesús López Aragón** - *IT Member* - [ilopez](ilopez@kea.mx)

## Licencia 📄

Este proyecto está bajo la Licencia (Tu Licencia) - mira el archivo [LICENSE.md](LICENSE.md) para detalles

