# Awesome Profile Cards
Desarrollo de una aplicación web de creación de tarjetas de visita personalizadas (Proyecto grupal del módulo 2 : JavaScript)

#### Descripción
El proyecto consiste en realizar una aplicación web que nos permite crear una tarjeta de visita personalizada. En la página web podemos introducir nuestros datos profesionales y obtener una vista maquetada con esta información


### Desarrollo
Durante el desarrollo de esta aplicación web se han utilizado las siguientes tecnologías:

- Uso avanzado de formularios HTML.
- Maquetación usando CSS avanzado, como Flexbox y Grid.
- Uso de mediaqueries para que el diseño sea adaptable al dispositivo usando la estrategia mobile first.
- Gestión de eventos en el navegador.
- Acceso y envío de datos a un servidor.
- Almacenamiento en local usando LocalStorage.
- Uso de git para el control de versiones del proyecto.
- Publicación del resultado en Internet usando GitHub Pages.


Para la realización de este proyecto se han seguido los siguientes hitos (genereales). La organizacón interna del equipo se ha sustentado en Trello. Se ha trabajado mediante **Sprints** semanales, para concluir finalmente con una **Demo** como entrega final:

- Desarrollo de la página de Landing.
- Desarrollo de una primera versión básica de la web, con la maquetación de la estructura básica (para desktop y móvil) que incluye el formulario con los colapsables y la vista previa de la tarjeta.
- Activación de la interacción del formulario: al modificar un campo del formulario, tanto del diseño de la tarjeta como de los datos de usuario se actualiza la vista previa.
- Creación de validaciones de datos del formulario.
- Creación de funcionalidad del botón de Reset: al clickar el LocalStorage debe limpiarse y el formulario debe volver a su estado inicial.
- Creación de la funcionalidad de compartir en Twitter, enviando primero los datos al servidor para obtener la URL para compartir.
- Creación de la funcionalidad de LocalStorage para que el contenido se almacene en el navegador.


La aplicación web cuenta con dos páginas: 

###### 1 Landing
![FireShot Capture 073 - 101880645-8acf3a00-3b93-11eb-8178-df25db8711d1 png (1920×881)_ - user-images githubusercontent com](https://user-images.githubusercontent.com/70572595/102081054-dc83f880-3e0f-11eb-8db3-eb42c3829515.png)


###### 2 Página de creación de tarjetas
![FireShot Capture 076 - 101880668-94f13880-3b93-11eb-9c02-362658d4f660 png (1920×1021)_ - user-images githubusercontent com](https://user-images.githubusercontent.com/70572595/102081055-de4dbc00-3e0f-11eb-949c-4b1001204459.png)
![FireShot Capture 079 - 101880671-96226580-3b93-11eb-874a-8ba2e3e89111 png (1920×1000)_ - user-images githubusercontent com](https://user-images.githubusercontent.com/70572595/102081059-dee65280-3e0f-11eb-9096-3b94f0ccb65b.png)
![FireShot Capture 082 - 101880673-96226580-3b93-11eb-9792-c572a03e1fe6 png (1920×795)_ - user-images githubusercontent com](https://user-images.githubusercontent.com/70572595/102081065-e0b01600-3e0f-11eb-9c07-953a742b97c6.png)

#### Composición del código:
##### HTML
Dividido en partials, haciendo referencia a las secciones del código como sigue:
- Footer.html: contiene el código referente al footer.
- Header.html: contiene el código referente al header.
- Generator-main.html: Contiene el código referente a la previsualización de la tarjeta y el formulario de selección de paletas.
  - Form.html: Contiene el código referente al formulario de introducción de datos de usuario.
  - Share.html: Contiene el código referente a la tercera sección colapsable, de creación de tarjeta y botón de compartir en Twitter.
  - Main.html: Contiene el código referente a la sección principal de la página de landing.
    - Main-benefits.html: Contiene el código repetido de la sección principal de la página de landing.
    - Card-generator.html: Contiene los includes de los partials anteriormente citados referentes a la página de creación de tarjeta.
    
- Index.html: Contiene los includes de los partials anteriormente citados referentes a la página Landing.

##### SASS: Dividido en partials
 __Core__: Contiene los partials de la hoja de reset CSS y las variables utilizadas por tratarse de código repetido, además contiene los keyframes de las animaciones existentes y mixins para los breakpoints del sistema de responsive.
__Layout__: Contiene los partials referentes al footer y el header.
__Pages__: Contiene los estilos correspondientes a las páginas existentes: index (landing) y generator (página de creación de tarjeta).
__Main.scss__: Contiene los imports de los partials anteriormente citados.
js: Dividido en partials:
-    **1. Main.js** : partial actualmente vacío preparado para funciones de la sección principal.
-   **2. Add-img.js**: Contiene el código de la funcionalidad de añadir imagen en el formulario y mostrarla en la previsualización.
-  **3. Collapsable.js**: Contiene el código referente a la funcionalidad para colapsar y desplegar los menús de la página de creación de tarjeta.
- **4. Card-dessign.js**: Contiene el código referente a las funcionalidades de paso de información y estilos de las paletas a la previsualización de la tarjeta.
-  **5. Localstorage.js**: Contiene el código referente a la funcionalidad de almacenamiento de la información introducida en el navegador.
- **6. Reset-button.js**: Contiene el código referente a la funcionalidad del botón de reset.

### Aprendizajes
![FireShot Capture 105 - Captura de pantalla 2020-12-14 a las 13 00 40 png (250x100) - ](https://user-images.githubusercontent.com/70572595/102080242-6af77a80-3e0e-11eb-8c2f-74e1e3c52930.png)
![FireShot Capture 108 - Captura de pantalla 2020-12-14 a las 13 00 49 png (2514×1414) - ](https://user-images.githubusercontent.com/70572595/102080071-1f44d100-3e0e-11eb-8e6b-e9a3910d7a6b.png)

### Arranque del proyecto:
Para instalar las dependencias

```
npm install 
```
Para arrancar el proyecto y probarlo en desarrollo a través de la URL '//localhost:3000/#/'
start
```
npm start
``` 
Para publicar el proyecto a producción
```
npm run docs
````

> **Equipo formado por**
Edurne Vila, Estíbaliz Barato, Marta Rey, Milda Grabyte y Yamira Martín formamos en su mometo el equipo de trabajo **< emyem >**.
Nuestra organizacion se ha basado en herramientas como Trello, Slack, Zoom y/o Meets para una establecer una comunicación diaria y efectiva. 
Logramos alcanzar los tres puntos que a continuación se señalan. 

![FireShot Capture 128 - Captura de pantalla 2020-12-14 a las 13 00 14 png (2522×1426) - ](https://user-images.githubusercontent.com/70572595/102079984-f6244080-3e0d-11eb-982e-4dff0e973c67.png)
Hecho con mucho 💜 por < emyem >

![FireShot Capture 114 - Captura de pantalla 2020-12-14 a las 13 01 06 png (2510×1412) - ](https://user-images.githubusercontent.com/70572595/102080113-2d92ed00-3e0e-11eb-91bd-3df8bcb42718.png)
