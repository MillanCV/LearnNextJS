# [Learn NextJS](https://nextjs.org/learn/foundations/about-nextjs?utm_source=next-site&utm_medium=homepage-cta&utm_campaign=home)

## Conociendo Next.js

### Next.js es un framework para React que permite manejar

- Interfaces de usuario
- Routing
- Data Fetching
- Renderizado
- Integraciones con servicios de terceros
- Infraestructura
- Rendimiento
- Escalabilidad
- Experiencia de desarrolle

### Next.js como React framework

Ofrece un conjunto de herramientas y configuraciones para React y estructuras
adicionales y optimizaciones.

## 1: Conociendo React

Cuando un usuario visita una web el servidor devuelve un HTML como index.html.

El navegador lee el HTML y construye el DOM.

El DOM es un objeto que representa los elementos HTML. Un puente entre el codigo
y la interfaz de usuario.

Un programador puede usar los metodos del DOM y un lenguaje como javascript para
atender a eventos de usuario y manipular el DOM, seleccionando, anadiendo,
actualizando y borrando elementos especificos en la interfaz de usuario.

### JSX

JSX es una extension de la sintaxis de JS que permite describir la UI con
sintaxis HTML.

#### Reglas

- Devolver un solo elemento (que puede contener otros, como &lt;div> o <>)
- Cerrar todas las tags (como &lt;img/>)
- camelCase

Los navegadores no entienden JSX. Es necesario traducirlo antes mediante
herramientas como Babel.

### Conceptos fundamentales

#### Components

Las interfaces pueden descomponerse en bloques llamados **componentes**. Estos
son reusables.

En React, los componentes son funciones.

#### Props

Los elementos HTML tienen atributos, una forma de pasarles informacion para
modificar su comportamiento. Cambiar el atributo src del elemento img hace que
cambie la imagen que muestre.

De manera similar, se puede pasar informacion como propiedades a los componentes
React. Son las **props**.

De forma similar a las funciones JS, se pueden disenar componentes que acepten
props que cambien el comportamiento del componente o lo que es renderizado en
pantalla.

Estas props se pasan de padres a hijos en un flujo de un solo sentido.

#### State

Mediante **state** y **event handler**s, React permite anadir interactividad.

React tiene un conjunto de funciones llamadas **hooks** destinadas a anadir
logica a los componentes, como **state**.

**State** es cualquier informacion en la UI que cambia con el tiempo, a menudo
activada por el usuario.

Por ejemplo, el hook useState() almacena el estado de una variable.

useState() devuelve un array. El primer elemento es el valor del estado. El
segundo elemento es una funcion para actualizar el valor.

El estado es inicializado y almacenado en un componente. La logica para
actualizarlo debe ser almacenada donde fue inicialmente creado.

## 2: From react to Next.js

`bash npm install react react-dom next`

### Como funciona Next.js

#### Desarrollo y produccion

En desarrollo Next optimiza para el desarrollador, incluyendo Typescript, ESlint, Fast Refresh...

En produccion optimiza para el usuario final.

De desarrollo a produccion hay tareas de compilacion, bundled, minifies y code split.

NextJS tiene un compilador desarrollado en rust que se encarga de estas transformaciones.
