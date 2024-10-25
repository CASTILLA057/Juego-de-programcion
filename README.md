# Juego-de-programacion

1. Las clases Utilizada para el programa:
Clase Personaje: Es una clase base que representa tanto a los héroes como al villano. Los atributos principales son:

nombre: nombre del personaje.
fuerza: la cantidad de daño que puede hacer con un ataque.
velocidad: una característica que podría afectar el turno, aunque en este código no se usa.
vida_hp: la salud del personaje. Si llega a cero, el personaje muere.
poder: una habilidad especial o descripción del poder del personaje.
ataques: una lista de los ataques que el personaje puede realizar.

Métodos principales de la clase Personaje: lo que le da vida al personaje y tenga una mejor mecanica en el combate.

-atacar(Personaje objetivo, int indiceAtaque): Permite que el personaje ataque a otro. Reduce la vida del personaje objetivo en función de la fuerza del atacante.
-estaVivo(): Devuelve true si la vida del personaje es mayor a 0, lo que indica que sigue en combate.
-mostrarEstado(): Muestra el estado actual del personaje, como el nombre y la vida.
-lase SuperHero y Villano: Son subclases de Personaje, es decir, heredan los atributos y métodos de la clase Personaje, pero pueden tener comportamientos adicionales o específicos.

2. Los metodos que se utilizaron fueron los siguientes:
Métodos sobrescritos (@Override) en SuperHero y Villano:
El método mostrarEstado() es sobrescrito para que además de mostrar el nombre y la vida, también se muestre el poder especial del personaje.

3. Funcionalidad del Juego

Creación de personajes:

Se crean 5 héroes (SuperHero[] heroes) con distintos atributos, ataques y poderes.
Se crea un villano poderoso (Villano villano).
Interfaz del juego:

El juego comienza mostrando el estado inicial de los héroes y del villano, usando mostrarEstado() para cada personaje.
Luego, el jugador debe decidir si atacar (a) o huir (h). Si huye, el juego termina.
Ciclo de combate:

Si el jugador decide atacar, el ciclo de combate comienza:
El jugador elige con qué héroe atacar.
Luego selecciona uno de los ataques disponibles para ese héroe.
El héroe seleccionado ataca al villano. La vida del villano se reduce según la fuerza del héroe.
Si el villano aún está vivo, realiza un ataque a cada héroe que siga en pie.
El ciclo se repite hasta que el villano o todos los héroes son derrotados.
Final del juego:

El juego termina cuando el villano es derrotado o todos los héroes son vencidos.
4. Escenario interactivo
El jugador interactúa con el juego usando el teclado para tomar decisiones, como seleccionar a qué héroe usar o qué ataque realizar.
Si las entradas del jugador son inválidas (por ejemplo, si se selecciona un número fuera de rango), se manejan errores como NumberFormatException para evitar que el juego se rompa y permitir que el jugador vuelva a intentarlo.

Nota:Este seria el paso a paso que manejamos en la creacion de nuestro juego,teniendo una forma dinamica y una seleccion de hasta 5 superheroes y un villano al cual nuestra mision es derrotarlo, pero tambien podemos salir derrotados de esta gran pelea todo va a estar concentrado en como el jugador idealiza sus jugadas para salir victorioso,solo queda decir ¡Buena suerte! en esta batalla.
