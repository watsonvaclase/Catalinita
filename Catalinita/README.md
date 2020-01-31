# Catalinita
Te presento a Catalinita: una niña muy lista y muy guapa a la que le encanta jugar y ayudar.

![Catalinita](./Catalinita.png)
<br>

## Catalinita te ayuda a probar la capacidad de hablar de tu TJBot
Si dudas de la capacidad de hablar de tu TJBot, Catalinita te saca de dudas. Ella verbalizará el texto que tú quieras.

Para poner en marcha el programa _Catalinita\_hablame.js_ sólo tienes que hacer cinco cosas:
1. Descargar el audio ![Noise.wav](./Noise.wav) y el programa ![Catalinita_hablame.js](./Catalinita_hablame.js) a la raspberrypi.
2. Ubicar los dos ficheros descargados (_Noise.wav_ y _Catalinita\_hablame.js_) en el directorio donde esté el programa _conversation.js_ del TJBot.
3. Asegurar que en ese directorio haya un subdirectorio llamado _node\_modules_. En caso negativo, ejecutar: <br>
_npm install_
4. Asegurar que en el mismo directorio exista y esté bien completado el fichero de credenciales _config.js_ 
5. Ejecutar: <br>
_sudo node Catalinita\_hablame.js "xxx"_ <br>
siendo _xxx_ el texto que quieras que Catalinita verbalice. <br>

(Si no oyes nada, pero no te sale ningún error por pantalla, prueba a conectar un altavoz con mini-jack usando un adaptador para el puerto usb. <br>
Si el altavoz distorsiona, prueba la misma solución.)<br>

## Catalinita te ayuda a probar la capacidad de escuchar de tu TJBot
Si dudas de la capacidad de escuchar de tu TJBot, Catalinita te saca de dudas. Ella repetirá todo lo que tú le digas.

#### Poner en marcha el programa _Catalinita\_lorito.js_
Sólo tienes que hacer cinco cosas:
1. Descargar el programa ![Catalinita_lorito.js](./Catalinita_lorito.js) a la raspberrypi.
2. Ubicar el programa descargado (_Catalinita\_lorito.js_) en el directorio donde esté el programa _conversation.js_ del TJBot.
3) Asegurar que en ese directorio haya un subdirectorio llamado _node\_modules_. En caso negativo, ejecutar: <br>
_npm install_
4. Asegurar que en el mismo directorio exista y esté bien completado el fichero de credenciales _config.js_ 
5. Ejecutar: <br>
_sudo node Catalinita\_lorito.js_

#### Usar el programa _Catalinita\_lorito.js_
Puedes interactuar con Catalinita diciéndole:
1. _Hola_: te saludará.
2. _Adiós_: se despedirá.
3. O cualquier cosa: te repetirá lo que te haya entendido. <br>

(Si _Catalinita\_lorito.js_ te funciona perfectamente, pero el programa _conversation.js_ del TJBot no te responde nada, recuerda que cuando uses el _conversation.js_ debes empezar cada frase que digas con el nombre del TJBot que hayas definido. Si no le has puesto ningún nombre específicamente, por defecto su nombre es Watson.<br>
Asegúrate de que el TJBot entiende bien el nombre que has elegido.)<br>

## Catalinita se sabe las tablas de multiplicar
Catalinita se ha aprendido las tablas de multiplicar de la 0 a la 20. Te las puede decir ella a ti, o te las puede preguntar para que tú se las digas a ella, a ver si tú también te las sabes.

¡No dejes de ver el vídeo para conocerla en acción!

[![Catalinita](./Catalinita_tablas_de_multiplicar_pelicula.png)](https://ibm.box.com/s/nkxo56m83rgzx36fkxftbrcqn55jp0lq)

#### Poner en marcha el programa _Catalinita\_tablas\_de\_multiplicar.js_
Si quieres que Catalinita te ayude a aprenderte las tablas de multiplicar, sólo tienes que hacer tres cosas:
1. Descargar el programa ![Catalinita_tablas_de_multiplicar.js](./Catalinita_tablas_de_multiplicar.js) a la raspberrypi.
2. Ubicar el fichero descargado (_Catalinita\_tablas\_de\_multiplicar.js_) en el directorio donde ya estés ejecutando satisfactoriamente el programa _conversation.js_ del TJBot o _Catalinita\_lorito.js_.
3. Ejecutar: <br>
_sudo node Catalinita\_tablas\_de\_multiplicar.js_

#### Usar el programa _Catalinita\_tablas\_de\_multiplicar.js_
Puedes interactuar con Catalinita haciéndole alguna de las siguientes preguntas:
1. _Dime la tabla del trece_. (En vez de trece, le puedes decir cualquier número del 0 al 20.) 
2. _¿Cuánto es nueve por siete?_ (En vez de nueve y siete, le puedes decir cualesquieras dos números entre el 0 y el 20.)
3. _¿Pregúntame todas las tablas?_ (Y te preguntará aleatoriamente la multiplicaciónun de dos números entre el 2 y el 10.)
4. _¿Pregúntame la tabla del ocho?_ (En vez de ocho, le puedes decir cualquier número del 0 al 20.)
5. _Otra vez_ (En caso de que le hayas pedido que te pregunte ella, para pedirle que te vuelva a preguntar con las mismas condiciones, puedes repetirle la pregunta o decirle simplemente _otra vez_.)

## Catalinita juega a "piedra, papel o tijera"
No pierdas la oportunidad de jugar con Catalinita a "piedra, papel o tijera". A ver cuántas veces te gana.

¡Mira el vídeo y verás cómo se enfada cuando pierde!

[![Catalinita](./Catalinita_piedra_papel_o_tijera_pelicula.png)](xxxx)

#### Poner en marcha el programa _Catalinita\_piedra\_papel\_o\_tijera.js_
Este programa es un poco más difícil de poner en marcha que los anteriores, pero no imposible.<br>
Para agilizar la conversación con Catalinita, los textos que ella verbaliza han sido generados previamente.<br>
Para que Catalinita pueda jugar contigo a "piedra, papel o tijera" tienes que hacer seis cosas:
1) Descargar todos los ficheros de la carpeta [Catalinita_piedra_papel_o_tijera](https://ibm.box.com/s/lyglhzt661lullh2awv49qv9bt523z5f) a la raspberrypi.
2. Ubicar todos los ficheros descargados en el directorio donde ya estés ejecutando satisfactoriamente el programa _conversation.js_ del TJBot o _Catalinita\_lorito.js_. Posicionarse en ese directorio.
3. Entrenar un modelo de Visual Recognition para enseñar a Catalinita a distinguir entre piedra, papel o tijera:<br>
3.1. Asegurar que la credencial del servicio Visual Recognition de Watson está correctamente introducida en el fichero _config.js_.<br>
3.2. Crear un modelo nuevo específico para este juego:<br>
_curl -X POST -u "apikey:xxx" \
--form "piedra_positive_examples=@piedra.zip" \
--form "papel_positive_examples=@papel.zip" \
--form "tijera_positive_examples=@tijera.zip" \
--form "negative_examples=@negativos.zip" \
--form "name=piepati" \
"https://gateway.watsonplatform.net/visual-recognition/api/v3/classifiers?version=2018-03-19"_<br>
siendo _xxx_ la credencial del servicio Visual Recognition.<br>
Después de un rato largo, el comando devolverá las características del modelo (también llamado clasificación) recién creado. Es importante apuntar el nombre otorgado a esta nueva clasificación. Ese nombre será algo como _piepati\_yyy_, y estará a la derecha del parámetro _"classifier_id":_<br>
3.3. Esperar hasta que el modelo esté listo. Esto es así cuando, al ejecutar:<br>
_curl -X GET -u "apikey:xxx" "https://gateway.watsonplatform.net/visual-recognition/api/v3/classifiers/piepati_yyy?version=2018-03-19"_<br>
el parámetro _"status":_ ofrece el valor _ready_.
4. Modificar la librería _node\_modules/tjbot/lib/tjbot.js_ para que el modelo de Visual Recognition que use Catalinita al jugar sea el recién entrenado, para ello:<br>
4.1. Buscar dentro de la librería la función _TJBot.prototype.recognizeObjectsInPhoto_. (Está alrededor del número de línea 920.)<br>
4.2. Dentro de esa función, en el párrafo donde se rellena la variable _params_, localizar la línea:<br>
_images_file: fs.createReadStream(filePath),_<br>
y añadir a continuación lo siguiente (incluyendo la coma final): <br>
_"classifier_id": "piepati_yyy",_<br>
4.3. Guardar los cambios hechos en el fichero y cerrarlo.
5. Instalar el paquete opn:<br>
_npm install opn_<br>
(Este paquete se utiliza para que Catalinita pueda abrir el navegador y mostrar lo que saca ella en cada tirada.)
6. Ejecutar: <br>
_sudo node Catalinita\_piedra\_papel\_o\_tijera.js_<br>
(Debes tener la precaución de cerrar todas las ventanas de las tiradas, cada vez que invoques el programa.)

#### Usar el programa _Catalinita\_piedra\_papel\_o\_tijera.js_
Puedes interactuar con Catalinita diciéndole simplemente "piedra, papel o tijera":
1. Ella te contestará: _venga, saca tú_.
2. Deberás enseñarle tu opción acercando tu mano a la cámara a un palmo de distancia. Para que el modelo entrenado funcione a la perfección, es conveniente que la cámara esté situada a la altura de tu cintura, y que detrás de ti haya una pared blanca, o por lo menos, que no haya nadie más, ni brazos, ni manos, ni piernas, ni caras.
3. Al mismo tiempo que tú sacas, Catalinita por pantalla mostrará lo que saca ella. 
4. Ella evaluará lo que tú has sacado, lo comparará con lo suyo y anunciará quién es el ganador. 

¡Ánimo y que tengas mucha suerte!

#### Más comandos útiles para gestionar la clasificación/modelo de Visual Recognition
Otra forma de extraer el _classifier\_id_ y el _status_ es obteniendo la información de todas las clasificaciones asociadas al servicio Visual Recognition que se esté usando. Para hacer esto usa el comando:<br>
_curl -u "apikey:xxx" "https://gateway.watsonplatform.net/visual-recognition/api/v3/classifiers?verbose=true&version=2018-03-19"_

Para evaluar la eficacia del modelo creado se puede intentar clasificar manualmente una imagen, para ello, basta con ejecutar:<br>
_curl -X POST -u "apikey:xxx" --form "images_file=@www"  --form "classifier_ids=piepati_yyy" "https://gateway.watsonplatform.net/visual-recognition/api/v3/classify?version=2018-03-19"_<br>
siendo _www_ el nombre del fichero jpg, con path completo, que se quiere someter a examen.

Como el número de modelos que se pueden tener en un servicio Visual Recognition es limitado, puede ser interesante borrar modelos que ya no se usen:<br>
_curl -X DELETE -u "apikey:xxx" "https://gateway.watsonplatform.net/visual-recognition/api/v3/classifiers/piepati_yyy?version=2018-03-19"_

#### Problemas comunes al usar el programa _Catalinita\_piedra\_papel\_o\_tijera.js_
Si tienes problemas, échale un ojo a los siguientes puntos:
1. Si dudas de las imágenes que capta tu TJBot, puedes ver las capturas en el directorio /tmp de tu raspberrypi.
2. Si ves que el modelo entrenado con las imágenes proporcionadas por Catalinita no se ajusta a tus necesidades, no dudes en incorporar en los ficheros _.zip_ más imágenes de cada tipo para enseñar a Catalinita a distinguir mejor entre piedra, papel o tijera.
3. Si al ejecutar _sudo node Catalinita\_piedra\_papel\_o\_tijera.js_ obtienes un error del siguiente estilo:<br>
<<<br>
verbose: TJBot initializing LED<br>
verbose: TJBot initializing microphone<br>
verbose: TJBot initializing servo motor on PIN 7<br>
2019-06-08 10:15:55 initInitialise: bind to port 8888 failed (Address already in use)<br>
/home/KKCHU/node_modules/pigpio/pigpio.js:11<br>
    pigpio.gpioInitialise();<br>
           ^<br>
Error: pigpio error -1 in gpioInitialise<br>
    at initializePigpio (/home/KKCHU/node_modules/pigpio/pigpio.js:11:12)<br>
    at new Gpio (/home/KKCHU/node_modules/pigpio/pigpio.js:25:3)<br>
    at TJBot._setupServo (/home/KKCHU/node_modules/tjbot/lib/tjbot.js:304:19)<br>
    at TJBot.<anonymous> (/home/KKCHU/node_modules/tjbot/lib/tjbot.js:71:18)<br>
    at Array.forEach (<anonymous>)<br>
    at new TJBot (/home/KKCHU/node_modules/tjbot/lib/tjbot.js:56:14)<br>
    at Object.<anonymous> (/home/KKCHU/ppt/ppt.js:46:10)<br>
    at Module._compile (internal/modules/cjs/loader.js:654:30)<br>
    at Object.Module._extensions..js (internal/modules/cjs/loader.js:665:10)<br>
    at Module.load (internal/modules/cjs/loader.js:566:32)<br>
    at tryModuleLoad (internal/modules/cjs/loader.js:506:12)<br>
    at Function.Module._load (internal/modules/cjs/loader.js:498:3)<br>
    at Function.Module.runMain (internal/modules/cjs/loader.js:695:10)<br>
    at startup (internal/bootstrap/node.js:201:19)<br>
    at bootstrapNodeJSCore (internal/bootstrap/node.js:516:3)_<br>
\>><br>
cierra todas las ventanas del navegador que tengas abiertas.<br>
Debes tener la precaución de cerrar todas las ventanas de las tiradas, cada vez que invoques el programa.

## Catalinita te ayuda con las matemáticas
Catalinita ha visitado a su amiga Hipotenocha en [ESTENMÁTICAS](http://nueva.estenmaticas.es/) y ha diseñado un chatbot para guiarte por todas sus posibilidades.<br>
Prueba [HipotenochaBot](https://assistant-chat-us-south.watsonplatform.net/web/public/d7639ece-5e29-490c-b304-ecc589e97933) o construye tu propio _HipotenochaBot_ siguiendo las instrucciones siguientes.

#### Poner en marcha tu propio _HipotenochaBot_
Para construir tu propio _HipotenochaBot_ tienes que hacer nueve cosas:
1. Descarga el json [Catalinita_HipotenochaBot.json](./Catalinita_HipotenochaBot.json) en tu PC.
2. Abre tu _panel de control o dashboard_ en [IBM Cloud](https://cloud.ibm.com), selecciona tu servicio _Watson assistant_ y lánzalo.
3. En los iconos de la izquierda, pulsa en el dibujito de _skills_.
4. Pincha en el botón _Create skill_ (¡OJO! si tienes ya cinco skills creados tendrás que borrar alguno).
5. Selecciona el tipo _Dialog skill_ (estará seleccionado por defecto).
6. Haz click en el botón _Next_.
7. Busca la opción _Import skill_ y pulsa sobre ella.
8. Pincha en el botón _Choose JSON File_, localiza el fichero json que descargaste en el paso 1 y haz doble click sobre él para seleccionarlo y cerrar la ventana.
9. Pulsa el botón _Import_.<br>
Después de un ratín, aparecerá entre tus skills, uno llamado _HipotenochaBot_.

#### Usar el chatbot _HipotenochaBot_
Nada más arrancar _HipotenochaBot_, ésta te saludará y se pondrá a tu servicio:
1. Escribe: _¿Qué sabes hacer?_.
2. Ella te mostrará una explicación de sus habilidades y te ofrecerá ayuda más detallada.
3. Escribe: _ok_.
4. Ella te enseñará todas las categorías que maneja y las palabras clave que puedes usar para buscar dentro de cada una de ellas. (Realmente puedes usar más porque hay muchos sinónimos definidos.)
5. Escribe: _me gustaría ver explicaciones de geometría para la ESO, por favor_.
6. Ella te ofrecerá las 15 URLs que cumplen el criterio _ESO geometría explicación_. (Son vídeos y paisajes de aprendizaje.)
7. Escribe: _ejemplos de recuperaciones de algebra de tercero de matemáticas aplicadas_.
8. Ella te dará todas las características de la única URLs que cumple el perfil _3º matemáticas aplicadas álgebra recuperación_. 
9. Escribe: _vídeos de la pregunta matemática de la aventura del saber_.
10. Ella te dirigirá al enlace con los vídeos de divulgación matemática que durante tres temporadas estuvieron emitiéndose en el programa _La aventura del saber_ de _La 2 de RTVE_. 
11. Escribe: _https://www.youtube.com/playlist?list=PLd2wVZS4p5o7cAWk1Kx8JmrFBkz29NZj4_.
12. Ella te dirá todo lo que sabe sobre esa url. (¿Quieres saber cómo acabar con los piojos matemáticamente? ¡Esta es tu ruta!)
13. Escribe: _Muchas gracias_.
14. Ella te responderá con un mensaje agradable, :). 

¡Ya no tienes excusa para no aprender matemáticas!

#### Claves para entender el diseño de _HipotenochaBot_
El algoritmo del diálogo de _HipotenochaBot_ está diseñado para realizar búsquedas por múltiples criterios entre los datos contenidos en una variable de tipo diccionario llamada _bluepages_.
Sirva de ejemplo de elemento contenido en ese diccionario el siguiente bloque:<br>
          {<br>
            "rama": "matemáticas, matemáticas académicas",<br>
            "ruta": "http://nueva.estenmaticas.es/videos-4o-eso-academicas",<br>
            "etapa": "ESO, Bachillerato",<br>
            "nivel": "4º",<br>
            "video": "vídeo",<br>
            "contenido": "explicación",<br>
            "comentario": "En el siguiente link podrás encontrar los vídeos de explicaciones numerados de 4º de ESO matemáticas académicas. Ten en cuenta que el temario ESTENMÁITCAS se imparte habitualmente en el siguiente orden: Estadística, Probabilidad, Geometría, Números, Álgebra y Análisis. http://nueva.estenmaticas.es/videos-4o-eso-academicas",<br>
            "area_de_conocimiento": "Estadística, Probabilidad, Geometría, Números, Álgebra, Análisis"<br>
          }<br>
<br>
Ese diccionario está relleno con los datos de la hoja Excel [Catalinita_HipotenochaBot_hoja_base.xlsx](./Catalinita_HipotenochaBot_hoja_base.xlsx).<br>
En esa hoja están las URLs objeto de búsqueda del chatbot. Las columnas son los distintos tipos de características por las que se puede buscar. En las filas de una columna concreta se pueden ver los valores claves que servirán para hacer las búsquedas de las URLs. <br>
Cada columna es una entidad del chatbot, cuyos valores corresponden a las claves referenciadas en su columna de la hoja Excel. Los valores de las entidades pueden tener sinónimos creados, por ejemplo, "primero" es un sinónimo de "1º".<br>
<br>
Dicho esto, encontrar la URL que cumple un determinado criterio, por ejemplo, que sea _de vídeos de explicaciones de cuarto de la ESO_, es lo mismo que encontrar bajo la columna _ruta_ de la hoja Excel la fila que contiene en la columna _etapa_ la clave "ESO", y además, en la columna _nivel_ la clave "4º", y además, en la columna _contenido_ la clave "explicación", y además, en la columna _video_ la clave "vídeo". Trasladándolo al chatbot, el objetivo sería encontrar el elemento del diccionario que cumpla que etapa=ESO y nivel=4º y contenido=explicación y video=vídeo.<br>
<br>
Este chatbot usa slots para dejar en variables los valores de las entidades detectadas en la conversación, pero no obliga a que estén rellenas.<br>
_HipotenochaBot_ es un valioso ejemplo del uso de SpEL expressions para manejar variables, arrays, añadir elementos, filtrar, buscar...<br>
Contiene además muchas _chit chat intents_ para hacer la conversación más humana.<br>
Introduce el concepto _confidence _ en los criterios de los diálogos para que sólo se entre en ellos si el grado de confianza de la intención detectada es mayor del 40%.<br>

