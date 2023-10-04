# Widget del Tiempo

A continuación, se presenta un código HTML que representa un widget del tiempo con información actual y pronóstico para varios días. Este widget está diseñado para mostrar el pronóstico del tiempo de Salta Capital, Argentina. Además, se utiliza un archivo de estilo CSS externo para dar formato y estilo al widget.

## Estructura del Documento HTML

El documento HTML está estructurado de la siguiente manera:

- `<!DOCTYPE html>`: Esta línea declara el tipo de documento y la versión de HTML utilizada.

- `<html lang="es">`: Define la estructura principal del documento HTML y especifica el idioma ("es" para español).

- `<head>`: Esta sección del documento se utiliza para incluir metadatos y enlaces a hojas de estilo externas.

  - `<meta charset="UTF-8">`: Define la codificación de caracteres utilizada en el documento como UTF-8.

  - `<meta http-equiv="X-UA-Compatible" content="IE=edge">`: Indica que el documento debe ser interpretado en el modo más alto de compatibilidad en Internet Explorer.

  - `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Configura la vista inicial para dispositivos móviles.

  - `<title>Weather Widget</title>`: Establece el título de la página como "Weather Widget".

  - `<link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">`: Agrega una fuente de iconos de Google.

  - `<link rel="stylesheet" href="style.css">`: Vincula una hoja de estilo externa llamada "style.css" para dar formato al widget.

- `<body>`: Contiene el contenido principal del widget.

  - `<div class="weather-container">`: Un contenedor principal que agrupa todo el contenido del widget.

    - `<div class="current">`: Representa la sección de información actual del tiempo.

      - `<div class="city">Salta Capital, Argentina</div>`: Muestra el nombre de la ciudad y el país.

      - `<div class="day">Now</div>`: Indica que se trata de la información actual.

      - `<div class="row">`: Contiene la información actual del tiempo, como temperatura y estado del cielo.

        - `<div class="icon">`: Muestra un ícono que representa el estado del cielo.

        - `<div class="info">`: Contiene información detallada, como temperatura y estado del cielo.

          - `<div class="temperature">`: Muestra la temperatura actual y mínima.

          - `<div class="status">Partially Cloudy</div>`: Indica el estado actual del cielo.

      - `<div class="more">`: Contiene información adicional sobre el tiempo actual, como velocidad del viento, probabilidad de tormenta e humedad.

    - `<div class="list">`: Representa la lista de pronóstico del tiempo para varios días.

      - `<div class="day">`: Cada día tiene su propio contenedor que incluye el nombre del día, el estado del cielo, la temperatura máxima y mínima.

## Estilos y Hoja de Estilo CSS

Para dar formato al widget, se utiliza una hoja de estilo CSS externa llamada "style.css". Los estilos incluidos en esta

# Explicación del Código CSS

A continuación, se presenta una explicación detallada del código CSS proporcionado:

```css
.material-icons {
  font-family: "Material Icons";
  font-weight: normal;
  font-style: normal;
  font-size: 24px; /* Tamaño preferido de los iconos */
  display: inline-block;
  line-height: 1;
  text-transform: none;
  letter-spacing: normal;
  word-wrap: normal;
  white-space: nowrap;
  direction: ltr;

  /* Soporte para todos los navegadores WebKit. */
  -webkit-font-smoothing: antialiased;
  /* Soporte para Safari y Chrome. */
  text-rendering: optimizeLegibility;

  /* Soporte para Firefox. */
  -moz-osx-font-smoothing: grayscale;

  /* Soporte para IE. */
  font-feature-settings: "liga";
}
```

- `.material-icons`: Esta regla CSS se aplica a elementos con la clase `material-icons`, que generalmente se utilizan para mostrar iconos en el texto utilizando la fuente de iconos "Material Icons".

  - `font-family: "Material Icons";`: Establece la fuente utilizada para los iconos.

  - `font-weight: normal;`: Establece el peso de la fuente como normal.

  - `font-style: normal;`: Establece el estilo de la fuente como normal.

  - `font-size: 24px;`: Define el tamaño preferido para los iconos.

  - `display: inline-block;`: Hace que los iconos se muestren en línea como elementos de bloque.

  - `line-height: 1;`: Establece la altura de línea a 1 para garantizar una alineación adecuada.

  - `text-transform: none;`: Desactiva cualquier transformación de texto, como mayúsculas o minúsculas.

  - `letter-spacing: normal;`: Define el espaciado entre letras como normal.

  - `word-wrap: normal;`: Establece el comportamiento de división de palabras como normal.

  - `white-space: nowrap;`: Evita el desbordamiento de texto al no permitir el ajuste de línea.

  - `direction: ltr;`: Establece la dirección del texto de izquierda a derecha.

  - Soporte de renderizado y suavizado de fuentes para diferentes navegadores web como WebKit, Safari, Chrome, Firefox y IE.

```css
body {
  font-family: Arial, Helvetica, sans-serif;
}
```

- `body`: Esta regla CSS se aplica al elemento `<body>` del documento HTML.

  - `font-family: Arial, Helvetica, sans-serif;`: Establece la fuente utilizada para el texto en el cuerpo del documento como Arial, Helvetica o una fuente genérica sans-serif en caso de que las fuentes especificadas no estén disponibles.

```css
.weather-container {
  width: 450px;
  margin: 100px auto;
  background-color: #333;
  color: white;
  padding: 10px;
  border-radius: 50px;
}
```

- `.weather-container`: Esta regla CSS se aplica a elementos con la clase `weather-container`, que representa el contenedor principal del widget del tiempo.

  - `width: 450px;`: Establece el ancho del contenedor a 450 píxeles.

  - `margin: 100px auto;`: Crea un margen superior e inferior de 100 píxeles y centra horizontalmente el contenedor.

  - `background-color: #333;`: Define el color de fondo como gris oscuro (#333).

  - `color: white;`: Establece el color del texto en blanco.

  - `padding: 10px;`: Agrega un espacio interno de 10 píxeles alrededor del contenedor.

  - `border-radius: 50px;`: Aplica un radio de borde de 50 píxeles para dar forma redondeada al contenedor.

Estos son los estilos clave en el código CSS proporcionado. Se utilizan para dar formato y diseño al widget del tiempo en el documento HTML. La clase `.material-icons` se utiliza para personalizar la apariencia de los iconos, mientras que las reglas aplicadas a `.weather-container` se utilizan para dar forma y estilo al contenedor principal del widget.
