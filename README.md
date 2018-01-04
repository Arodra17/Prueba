# Prueba
La prueba la he realizado en un único archivo HTML, en el cual he incluido los códigos correspondientes de Javascript y CSS, con el fin de simplificar su ejecución.
Para ejecutar dicho arhivo basta con abrirlo como un documento normal, el navegador elegido lo ejecutará y nos mostrará directamente un mapa de Google mostrando la ubicación preestablecida en Tecnosylva.
En la cabecera podemos apreciar dos cuadros, inputs. 
El primero de ellos, a la izquierda es un buscador de localizaciones, si escribimos alguna localización existente y pulsamos en buscar localización, automáticamente nos mostrará dicha ubicación en el mapa, añadiéndole un marcador y el tiempo actual en un infowindow. De no escribir una localización real, saltará un alert al pulsar localización, avisándonos sobre la falsa localización introducida.
En el segundo cuadro, podemos ver un select, en el cual he metido una lista de clientes con unas coordenadas fijas,  por lo que al seleccionar un cliente y pulsar en el botón buscar cliente, automáticamente nos llevará a su ubicación. En esta lista y por defecto podemos ver que muestra Inicio y si seleccionamos esta opción nos retorna a Tecnosylva. Siempre al seleccionar un cliente o la posición inicial, nos mostrará el tiempo.
Para poder añadir cualquier marcador en todo momento y ver el tiempo actual en esa zona, sólo tenemos que pulsar el botón derecho de nuestro ratón, automáticamente colocará sobre el mapa un marcador y con él se abrirá un infowindow mostrando el tiempo de esa zona.
Para manejar el mapa, se usaría como cualquier mapa de Goolge o el mismo Google Maps.

Dentro del código, podemos ver que están los estilos, en lso que se definen el tamaño de mapa, los controles y los tamaños y colocación de los cuadros de los dos tipos de búsquedas.
En el cuerpo, defino los dos cuadros de búsqueda, tanto el select como el de búsqueda directa de una localización. También creo las diferentes funciones, como pueden ser getWeather con la que a través de Ajax hago la llamada al servicio de metereología de OpenWeather. 
También defino la función initMap con la cual añdo el comportamiento de las búsquedas y el comportamiento del botón derecho del ratón.
Si avanzamos vemos como con el método placeMarkerAndPanTo colocamos el markador al pulsar botón derecho y hacemos la llamada a getWeather.
con dos métodos más: geocodeLatLng y geocodeAddress damos función a las búsquedas. El primer método es para la búsqueda indirecta de clientes, empleando coordenadas y el segundo método es para hacer na búsqueda de localizaciones, a través de una dirección.
