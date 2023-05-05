# ejemplo-react
Demo react

EXPLICACIÓN DEL COMPONENTE SQURE
El componente Square es una función que devuelve un botón con una clase "square" y un valor que se pasa a través de la propiedad "value". Además, se pasa una función "onSquareClick" que se ejecutará cuando se haga clic en el botón.


BOARD
El componente Board es una función que contiene nueve instancias del componente Square organizadas en tres filas. También tiene un estado "xIsNext" que indica de quién es el turno y un estado "squares" que contiene el estado actual del tablero. Cuando se hace clic en un cuadrado, se llama a la función "handleClick" para actualizar el estado del tablero y el estado del turno. También se verifica si hay un ganador utilizando la función "calculateWinner".


GAME
El componente Game es el componente principal que contiene el estado completo del juego. Tiene un estado "history" que contiene un array de todos los estados del tablero anteriores, y un estado "currentMove" que indica el movimiento actual. Cuando se realiza un movimiento, se llama a la función "handlePlay" para actualizar el historial y el movimiento actual. También hay una función "jumpTo" que se llama cuando se hace clic en uno de los movimientos anteriores en el registro de movimientos.


CALCULATEWINNER
Por último, la función "calculateWinner" comprueba si hay algún ganador del juego utilizando una matriz de combinaciones ganadoras posibles. Si encuentra una combinación ganadora, devuelve el símbolo del ganador (X o O), de lo contrario devuelve null.