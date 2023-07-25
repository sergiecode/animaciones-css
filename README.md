![animaciones y keyframe en css](https://raw.githubusercontent.com/sergiecode/animaciones-css/master/01.jpg)

[Video ejemplo animacion (corto)2](https://github.com/sergiecode/animaciones-css/blob/master/02.mp4)

[Video ejemplo animación (corto)3](https://github.com/sergiecode/animaciones-css/blob/master/03.mp4)

[Video ejemplo animacion (corto)4](https://github.com/sergiecode/animaciones-css/blob/master/04.mp4)

[Video ejemplo animación (corto)5](https://github.com/sergiecode/animaciones-css/blob/master/05.mp4)



# Tutorial de Animaciones CSS con @keyframes

En este tutorial, aprenderemos cómo utilizar `@keyframes` en CSS para crear animaciones personalizadas. Las animaciones CSS son una forma poderosa de mejorar la interactividad y la experiencia del usuario en tu sitio web. Utilizando `@keyframes`, podemos definir varios estados de animación y aplicarlos a elementos HTML.

## Introducción

Las animaciones CSS permiten cambiar gradualmente los estilos de un elemento en un período de tiempo. `@keyframes` es una regla en CSS que define los estilos de animación en diferentes puntos clave durante la animación.

## Preparación

Antes de comenzar, asegúrate de tener un archivo HTML y un archivo CSS vinculados correctamente. Puedes hacerlo con las siguientes líneas de código en tu archivo HTML:
```
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tutorial de Animaciones CSS</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <!-- Tu contenido HTML aquí -->
</body>
</html>

```

## Creando la animación

Para crear una animación con `@keyframes`, sigue estos pasos:

1.  Abre tu archivo `styles.css`.
2.  Definiremos una animación que haga que un elemento se mueva de izquierda a derecha y cambie de color.
3.  Utilizaremos el nombre `slideAndColor` para la animación.

```
@keyframes slideAndColor {
  0% {
    transform: translateX(0);
    background-color: red;
  }
  50% {
    transform: translateX(200px);
    background-color: blue;
  }
  100% {
    transform: translateX(400px);
    background-color: green;
  }
}

```

En este ejemplo, hemos definido tres puntos clave en la animación (`0%`, `50%`, `100%`). Cada punto clave especifica cómo debe lucir el elemento en ese momento particular de la animación.

## Aplicando la animación

Ahora que hemos creado la animación, aplicaremos esta animación a un elemento en nuestro archivo HTML.

```

`<!-- Dentro del body de tu archivo HTML -->
<div class="animated-box"></div>` 

```

`/* styles.css */

```

.animated-box {
  width: 100px;
  height: 100px;
  background-color: red;
  animation: slideAndColor 3s infinite;
}` 

```

Hemos creado una caja (div) con la clase `animated-box` y le aplicamos nuestra animación `slideAndColor`. La animación durará 3 segundos y se repetirá infinitamente (`infinite`).
