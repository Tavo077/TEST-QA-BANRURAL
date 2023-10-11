Prueba en el desarrollo "Adivina tu numero" 

Analisis Caja negra: 
    - Se realizo el siguiente analisis realizando las siguientes validaciones sobre el funcionamiento en la vista de usuario

    - Se observa que el diseño de la página es muy simple, pero en los requerimientos no se detalla un diseño en especifico lo cual no se contempla ninguna corrección del mismo. 
 
 Validaciones de entrada de datos: 
    - Se valida en el sistema que el campo no acepta números con decimal ( No corregido )
 
    - Se valida en el sistema que el campo no acepte valores tipo caracter (No corregido)
 
    - Acepta valores menores a 0 (No corregido)

Analisis Caja blanca:

Problema:
    - Realizando las diferentes pruebas, se encontro que no se tenia el rango adecuado de numeros aleatorios
Correccion: 
    - Se corrigió agregándole el numero 100 + 1 para que se cumpla con el requisito que sea un rango de 1 a 100

Problema:
    - La constante ATTEMPS tiene = 5 lo cual es incorrecto 
Correccion:
    - Se corrigio colocando el dato correcto el cual es 10 

Problema:
    - Se encontro una falta en la definicion de la variable lowOrHi
Correccion:
    - Se debe agregar un punto antes de "lowOrHi" para seleccionar el elemento con la clase "lowOrHi"
 
Problema:
    - Se encontró en la línea 97 que en el evento addeventListener esta escrita de forma incorrecta
Correccion 
    - Se corrigio el nombre del evento addEventListener

Problema:
    - Se encontró en el evento addeventListener en la función setGameOver está escrita de forma incorrecta
Correcion:
    - Se corrigio el nombre del evento addEventListener

Problema:
    - En la funcion resetGame no tenia bien definida el rango correcto del nuevo numero aleatorio
Correccion:
    - Se agrego 100 + 1  para lograr generar un nuevo numero aleatorio en el rango correcto

Problema:
    - Se encontro las siguientes faltas en la funcion checkGuess
        - Los colores definidos en cada respuesta estan colocados incorrectamente 
Correcion:
        - Se corrigio los colores a cada respuesta de la funcion checkGuess segun el requerimiento
        Si el valor ingresado por el usuario es mayor o menor que el número objetivo, se muestre el mensaje en color negro.
        Si el usuario supera los 10 intentos, se muestre el mensaje en color rojo.
        Si el usuario adivina el número, se muestre el mensaje en color verde.

Problema:
        - No se cuenta con las validaciones que se encargan en permitir el ingreso unicamente de numeros enteros
Correcion:
        - Se agrega una nueva validacion la cual condiciona el ingreso de numeros enteros unicamente
        En esta modificación, hemos agregado dos condiciones adicionales a la validación:
        userGuess <= 0: Esto evita que se ingresen números negativos o cero.
        userGuess > 100: Esto evita que se ingresen números mayores que 100, ya que el rango válido es de 1 a 100.



