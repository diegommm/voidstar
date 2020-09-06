# void*

[[_TOC_]]

## Introducción

Me dispongo a explicar desde un punto de vista existencialista ciertos
conceptos básicos de programación y finalizar con una tesis acerca de la
depresión y el suicidio. No pueda tomarse este texto como nota suicida, siendo
demasiado trabajo, pero habiéndolo considerado algunas veces desistí porque
prefería programar. Que sería algo así como decir que me entusiasmé con la nota
suicida y la satisfacción de expresar mis sentimientos de forma escrita hizo
decaer el entusiasmo inicial. Es como decir que escribir hubiera evitado que
Hemingway se disparara en la cabeza o que Terry A. Davis se tirara a las vías
del tren. No siempre funciona, pero siempre es necesario, aún si tuviera el
efecto contrario.

### Títulos alternativos

Un título alternativo para este texto podría ser `Programación para suicidas`, y
sería bastante descriptitvo y llamativo, tal vez acertado, pero prefiero
reservar el drama para la vida. O también `Existencialismo para programadores` o
incluso `Cómo reflexionar sobre tu profesión, cualquiera sea, te puede permitir
justificar tus tendencias suicidas`.

## Los lenguajes de programación son lenguajes

En este sentido, cabe aclarar que escribir en algún lenguaje de programación no
es menos expresivo que escribir poemas en español o en cantonés. Es falso el
preconcepto de que quienes programan son discapacitados emocionales,
completamente privados de los sentimientos más profundos como el amor, la
repugnancia o la soledad. Es innegable que muchos programadores no son muy
talentosos pero sí trabajan de ello suficientemente bien y aún así nunca llegan
a hacer algo realmente bueno, como quienes tuvieron la desgracia de programar MS
Internet Explorer (y caer en la deshonra); pero qué podríamos decir del autor de
_El Alquimista_. Si hablamos de suicidio, es posible que los árboles talados
para recibir en su celulosa la tinta de ese texto hubieran salvado su destino de
haber estado consciente de él. Ah, un _seppuku_ forestal.

No obstante, ambos son _productos_ muy difundidos y conocidos. Productos
comerciales, pésimos, populares y que inexplicablemente siguen en circulación.

A menudo es más fácil coincidir en qué obra es mala que en cuál es buena. Y lo
digo así, de forma amplia, incluyendo en la palabra "obra" tanto textos
literarios como programas de computadoras. Todos sabemos que Internet Explorer
es pésimo; todos sabemos que cualquier forma de expresión de Coelho es una
manifestación paroxística de la estupidez y la superficialidad New Age. Incluso
quienes solo llegamos a leer un par de capítulos (y a mucha honra).

Lo mismo pasa con los programas: uno dirá que el kernel de Linux es una obra
maestra, otro argumentará que es _GNU/Linux_ sin ninguna conescuencia, otros
dirán que es un monolito innecesario de miles de millones de líneas de código y
que prefieren micro kernels.

## Punteros

Un puntero es una variable que guarda una posición de memoria. A los fines
prácticos, vamos a decir que un puntero es algo así como una tarjeta de
presentación, en la que encontraremos no a quien ella presenta sino dónde
encontrarlo. Ahora, un programador ávido de explotar esta analogía simplista
podría aclarar que también pueden existir punteros a punteros, que sería como
hablar de una tarjeta de presentación que presenta tarjetas de presentación.
Pero no es el objetivo entretener a este pequeño gran matón de la internet.

En efecto, tanto un puntero como una tarjeta de presentación son _referencias_ a
otra cosa, y a priori no podrían parecer muy útiles, ya que con una tarjeta de
presentación no puedo solucionar mi problema del reloj que se me rompió y con un
puntero solo no puedo hacer mucho más tampoco. En un puntero existe una
dirección de memoria, en la tarjeta de presentación, la dirección del relojero.

Dependiendo del lenguaje de programación, podrían realizarse muchas operaciones
con un puntero, pero sin duda alguna la más importante y la principal es la
operación de _desreferenciación_, lo que es, acceder a aquella información que
existe en la posición de memoria que tiene guardada, sea lo que sea. Una
operación similar en nuestra analogía es la de presentarse en el domicilio del
relojero. Desreferenciar un puntero es trasladarse hasta su dirección de memoria
y acceder a ella. Desreferenciar la tarjeta de presentación, trasladarse hasta
la dirección de quien presenta.

Asumiendo que pudiéramos llegar a la dirección del relojero sin mayores
problemas podríamos encontrarnos con problemas más graves. Muy graves. Y voy a
dar un ejemplo que me aterrorizaría que me sucediera si me pasara a mí al llegar
a la dirección del relojero que encontré en la tarjeta de presentación.

En la tarjeta de presentación aparece una fotografía del local comercial del
relojero. Tiene un cartel con tipografía Serif al estilo Times y tonalidades
marrón claro con detalles negros, muy clásico y evocador de un estilo inglés _à
la_ Big Ben. La tarjeta es de un papel de cartulina mate de buena calidad para
convencer a los snobs que llevarán sus relojes innecesariamente caros que en ese
lugar tomarán en serio sus fantasías y los harán jugar. "Clásico". Pero al
llegar a la dirección que indica la tarjeta me encuentro con un lugar abandonado
hace mucho tiempo. Mucho tiempo. Reviso la tarjeta, busco el cartel en la
fotografía y compruebo que se ve muy parecido a aquel cartel asediado por el
tiempo y por una intemperie que jamás esperó ver. Esta imagen _corrupta_ me
provoca todo tipo de pensamientos que fluyen en mi mente de forma que no puedo
controlar: ¿por qué la tarjeta está tan nueva y el lugar tan derruído? ¿quién
imprimió esta tarjeta? ¿cómo fue que llegué a recibirla? Cuestiono mi memoria.
Cuestiono lo que veo. Cuestiono mi concepción de la realidad: ¿acaso me fue
enviada esta tarjeta desde un pasado donde intentaban avisarme de algún peligro
relacionado con el viaje en el tiempo? Después de todo, es una relojería...

Lo más lógico es que entraría en _pánico_.

Del mismo modo, intentar desreferenciar un puntero que apunta a una posición de
memoria donde ya no está guardado algo que esperaría encontrar (como un relojero
en la analogía) provoca que algunos lenguajes de programación o sistemas
operativos entren en _pánico_ debido a que esa memoria está _corrupta_. Las
palabras resaltadas son literalmente las utilizadass en programación para estas
condiciones.

## Tipos de datos

Un tipo de dato es una abstracción de alguna idea que contiene un estado y
posiblemente también un comportamiento. Un tipo de dato puede ser tan abstracto
como se quiera. Por ejemplo, podemos hablar de un tipo de dato que se llame
"tarjeta de presentación" y que tiene la capacidad de guardar una dirección de
alguien y parte de su comportamiento podría ser "amarillentarse con el tiempo".
En el ejemplo que venimos tratando, es un comportamiento que yo hubiera esperado
de esa tarjeta de presentación y que hubiera esperado que esté presente. Pero
esa tarjeta estaba como nueva a mi parecer. Mi expectativa no encajó con lo
observado y entré en pánico cobardemente sin siquiera detenerme a pensar que el
dueño de la relojería gastó tanto dinero en la calidad de ese cebo de snobs que
terminó por quebrar y lo que terminó por perdurar más que su trabajo como
relojero es una fútil expresión de una sociedad eminentemente frívola y
desprovista de una justificación de ser más que la de procurar los mejores
adornos para su propio funeral. Bueno, también hay que resaltar la labor de los
trabajadores de la imprenta y de los productores de insumos.

De hecho, podría decirse que la industria de la publicidad, imprenta y afines es
la más exitosa de nuestros tiempos. Más aún, sería injusto continuar sin
resaltar también la labor de los trabajadores de las imprentas y empresas
publicitarias, quienes sostienen de forma exclusiva el mérito de haber logrado
que Coelho llegara a tener best-sellers. Lo mismo valdría, mutatis mutandis,
para MS Internet Explorer y gran parte de los productos informáticos que
salieron de un lugar conocido como Redmond.

Asimismo, muchos lenguajes de programación tienen _decoraciones_ con las cuales
adornan sus declaraciones de tipos de datos. Algo así como: "Háganse las
tarjetas de presentación", decorado con "que no estarán vivas". Aquí, lo
principal es nuestra oración principal que habla de algo nuevo que vamos a
crear, las tarjetas de presentación, y lo secundario es una oración subordinada
que aclara que no estarán vivas. Ahora, nótese la solemnidad abrahámica que
tinta estas declaraciones. Esta es una forma en que los programadores se
reservan una cuota de grandilocuencia para expresar a sí mismos y dentro de la
sociedad secreta de los animalillos de su tipo que tienen poderes sobrenaturales
para crear lo que sea. Un programador dice: "hágase un desastre" y a los pocos
días sale un prototipo de sistema operativo llamado QDOS (Quick-and-Dirty
Operative System), que sentará las chuecas bases y futuros defectos de todas las
versiones de Windows.

A los ojos de un humano regular sería raro pensar que una tarjeta de
presentación esté viva, lo cual haría completamente redundante tener que
declarar que una tarjeta de presentación efectivamente no _debería_ estar viva.
Al menos, es la esperanza que siempre albergamos en nuestros corazones. Eso
sería aterrador.

Pero si tenemos en cuenta la pomposa jerga del programador, hay que pensar como
un dios. Un dios capaz de crear tarjetas de presentación, que pueden o no estar
vivas. Después de todo, un programador paranoico podría crear un juego que trate
de tarjetas de presentación asesinas que buscan, sobre todo, llenar nuestras
billeteras y bolsos con una fuente inagotable de entropía. Distópico.

Pero bajemos de ese pedestal a este vulgar bípedo. Un programador es tanto un
dios dentro de sus programas como lo es un escritor dentro de sus novelas. En
este sentido, su poder es tan vasto e inalcanzable como imaginario. Como
cualquier dios, abrahámico o no. O como cualquier escritor, de evangelios o no.
Ningún Coelho debería tener poder más que en sus chatos e insípidos clichés.
Ningún Steve snob debería tener tanto poder como para obligar a niños a trabajar
en una mina de litio para fabricar baterías para sus productos electrónicos.

Así, pues, contribuyo a la concepción de que los lenguajes de programación son
también lenguajes o idiomas, donde se puede escribir "Mein Kampf" vs. "Philosophiæ
Naturalis Principia Mathematica"; una evangelio, corán, talmud, bhagavad gita u
otro texto sobre supersticiones varias vs. el Manifiesto Surrealista de André
Breton.

## Decoradores perniciosos

Algunos lenguajes de progamación intentan ser tan útiles que se exceden en la
capacidad de especificar decoradores. Por ejemplo, un lenguaje podría permitir
decir que "dado un tipo de dato que representa algo que está vivo", entonces
podríamos decir si este tipo de organismo es procariota o eucariota. En caso de
no ser un organismo vivo, podría ser un mineral o elemento químico en estado
puro. Y esto parecería ser muy útil, especialmente para lenguajes de
programación que estuvieran orientados a ese tipo de tareas científicas, salvo
que estos lenguajes de programación intentan "facilitar" tareas que
supuestamente no necesariamente tratan con este dominio de la información. Por
ejemplo: si quiero modelar una tarjeta de presentación: ¿de qué me servirían
todos esos excesivos y caros decoradores que especifican que, dado un ser vivo,
este sería procariota, eucariota, chordata, mamífero, primate, hominidae, etc.?

Para ejemplificar este exceso de locuacidad (en inglés encontrado a menudo como
`verbosity`) pongamos el ejemplo de un lenguaje de programación infamemente
popular: Java. Aquel programador que haya leído hasta este párrafo habrá
entendido qué cosa voy a nombrar a continuación. Es su destino. No debería
resistirse a aceptarlo. Estaría mal que lo intentara. Él sabrá que *Java está
mal*, desde su concepción. Al igual que C++ y tantos otros tristes ejemplos.

Antes de empezar a increpar a los java-users quisiera aclarar algo muy abstracto
que debemos considerar previamente antes de entrar de lleno en el ejemplo que
quiero presentar: el concepto de _void_.  Voy a realizar algunas aclaraciones
para los no angloparlantes primero. La palabra _void_ del inglés es a menudo
traducida al español como _vacío_. En este respecto hay que hacer un paréntesis
existencial para explicar la diferencia entre esta traducción enciclopedista y
el significante que persigue el concepto que necesitamos adquirir para entender
este elusivo idioma de los programadores, tan anglo-amantes.

En programación, hablamos de que algunos tipos de datos están _vacíos_, en
inglés _empty_, cuando se refieren a _ideas_ que significan en el fondo alguna
especie de _acumulador_ de elementos de una misma especie (sea cual fuere la
especie en cuestión), y cuyo estado pudiera luego descomponerse en cada uno de
los estados anteriores que le precedieron. El _acumulador_ en sí es una materia
de estudio y discusión donde algunos se sacan los ojos, perdiendo la visión del
objetivo general: la felicidad del ser humano y la satisfacción de todos los
seres vivos. Ja, ja, ja, Nótese tanto lo correcto de la expresión previa según
la R.A.E. como lo sarcástico de la misma. Son súper importantes las
matar gente.

Por el contrario, un tipo de dato relacionado de alguna forma con el primordial
_void_ es un animal distinto y difícil de domesticar. Void en sí es traducido
muchas veces según adeptos de la R.A.E. (nótese la excesiva puntuación) como
_vacío_. Pero el tipo _void_ encierra en sí una sustancia mucho menos tangible
que la ausencia de alguna sustancia específica: representa en sí mismo la
ausencia de sustancia cualquiera, de forma intrusiva en nuestros pensamientos,
rebuscando en cualquier rincón de existencia al que nos aferremos. Pregúntenle a
una persona que nació ciega qué es lo que ve con sus ojos. Tan solo el ejercicio
de pensar hacerlo debería hacerles reflexionar a ustedes, seres privilegiados,
acerca de sus _privilegios_.

Lo que quiero transmitir es que existe un _vacío_ más profundo que la ausencia
de cosas.

Eso es _void_.

## Puntero a relojero

No sé si ya lo aclaré, pero muchas veces se asocia el concepto de _puntero_ con
el carácter asterisco (_*_) precediendo o antecediendo un tipo de dato. Si no lo
hice, denle la bienvenida.

El significado de tal adorno sobre un tipo de dato es especificar que aquello
que va a ser guardado en tal o cual variable no es el estado en sí de una
instancia específica (o existencia, o vida) de un cierto tipo de dato, sino que
tiene la capacidad de _referenciar_ un elemento de tales características.

Ahora podríamos construir algo un poco más elaborado en base a los conceptos que
definimos: una "tarjeta de presentación" es un puntero a "presentado", donde
"presentado" es aquello a lo que la tarjeta intenta describir, tanto en su
ubicación como en sus capacidades.

Por ejemplo, la tarjeta que recibí no solo tiene una dirección (la dirección del
local comercial del relojero) sino que también tiene ciertas capacidades
específicas (aquello que es apuntado puede arreglar relojes). De este modo,
podemos entender que un _relojero_ es una _persona_ que es capaz de cambiar el
estado de un _reloj_ desde un estado _averiado_ a un estado _funcional_.

Podemos, entonces, identificar las siguientes elementos de interés en nuestro
modelo de la realidad que nos interesa:
1. Reloj. A su vez, un reloj puede estar en estado:
  1. Averiado (necesita ser arreglado).
  1. Funcional (no necesita ser arreglado).
1. Persona. A su vez, una persona puede ser:
  1. Relojero (puede arreglar un reloj).
  1. No relojero (no puede arreglar un reloj, al menos en general).

Ese es nuestro modelo. Lo que nosotros tenemos es:
1. Un _reloj_, que se encuetra en estado _averiado_.
1. Una tarjeta de presentación, que apunta a _relojer_ (que podría cambiar el
   estado de nuestro reloj a _funcional_).

Una posible resolución posible es:
1. Llevar con nosotros el _reloj_.
1. Desreferenciar la tarketa de presentación del _relojero_.
1. Hacer que el _relojero_ cambie el estado de nuestro _reloj_ desde su actual
   estado _averiado_ a _funcional_ (nótese que hablamos de "hacer que lo haga",
   ni siquiera decimos que vamos a pagar por ello. Podríamos amenazarlo de
   muerte para que lo hiciera y la solución sería igualmente válida según
   nuestro modelo. Lo único que nos interesa es arreglar el maldito reloj).

## The Big Void

Hermosa la analogía que venimos amasando. Espero que se haya entendido porque
ahora nos va a ocupar una abstracción existencialista a la altura de la obra de
Sartre. Y deprimente, filosófica, testaruda. No solo Sartre, sino también
Hemingway, Camus, Dostoievski, Poe, Dante y todos los escritores malditos que
quisieran ustedes invocar.  ¿Recuerdan el concepto de _void_? ¿Pensaban que
_void_ representaba una misma entidad, si es que alguna entidad fuera
representada por _void_?

No.

Y la respuesta no existe tanto como no hay pregunta que fuera a caber a la
interrogante de fondo. No existe una misma interpretación de _void_, porque
_void_ es un concepto filosófico por el que tanto Heidegger como Popper, Bohr,
Bunge, Schoppenhauer, Leibniz, Nietzsche, Bertalanffy o quien se les fuera a
ocurrir se ocuparon. Y ninguno tuvo una visión acorde a otro del todo.

No hay un _void_ universal. Y, aún así, tenemos un _puntero a void_ en muchos
lenguajes, cada uno siguiendo una rama filosófica específica preconcebida o una
propia. No es importante, después de todo, _void_ es un concepto superior a
cualqueira de ellas.

Puntero a void es algo más profundo que void en sí. Es algo que referencia a
algo que no somos capaces de describir en un lenguaje coloquial común y, aún
así, tiene tanta relevancia concreta su entendimiento que ustedes o yo no
podríamos compartir esta conversación innecesaria sobre _void_.

Si llegaron a este punto de la lectura, lo cual no lo recomendaría, y todavía no
dudan de su identidad es porque todavía no se cuestionaron lo suficiente el
precepto anti-rector de _void_. Este concepto es tan subversivo que provocó
demasiados pleitos e incluso al menos una muerte que sea de mi conocimiento.
Para no generar más controversia no mencionaré el caso que conozco. Mentira. Es
solo para hacerme el misterioso.

_void_ es parte de la identidad intrínseca de nuestro universo. Algunos
filósofos consideran que _void_ lo es todo y otros que es la nada y, aún otros
más, que _void_ es algunas cosas pero no otras. Cada uno tiene sus razones. Pero
no nos quedaremos en la conformidad nebulosa de _void_ sin decir nada acerca de
los angustiosos e intrincados intentos de entender _void_ dentro de la
programación.

Mencionaré lo siguiente y espero que se queden a cuestionar tan fuertemente lo
que diré que dejarán de leer lo que diga solo para gritarle a una pantalla o
papel donde estén leyendo para argüir en contra y, al mismo tiempo, a favor de
lo que fuera a decir. Y esto debería quitarles el sueño, se los advierto.

El ejemplo que tomaré es del lenguaje de programación llamado, a secas, "C": un
punterpo a _void_ es un puntero a cualquier cosa.

Espero el cuestionamiento...

¿Acaso como ninguna entidad en específico puede ser _void_ entonces cualquiera
de ella puede ser _void_ en alguna instancia que referencie a _void_? Eso
significaría que cualquier entidad en específico es tan válida como cualquier
otra. Nadie es especial. Somos todos polvo de estrellas. Como dice un filósofo
(y repitieron en una serie famosa): nadie existe a propósito. No existe nada que
yo pueda _hacer_ o _ser_ para dejar de ser referenciado por un arbitrario
_puntero a void_. Ni siquiera _dejar de ser_. Porque recuerden que incluso _no
siendo_, como es el caso de las tarjetas de presentación asesinas, podrá existir
un _puntero a void_ que apunte a alguna de aquellas entidades.

Y es en esta asfixia cosmogónica autoritaria de _void_ que uno podría decir con
toda justicia (si tal cosa existe o no existe, sea como fuere):

```life
    Déjenme no ser.
```

#vimft: formatoptions=jtcqn textwidth=80
