#Read me
Aplicar el algoritmo de Luhn para informarle al usuario si el número que ingresó es el de una tarjeta de crédito válida

#Reglas
 El usuario no puede ingresar campos vacíos.

#Pseudocódigo de la solución propuesta

Prompt solicitando el número de tarjeta
Mandar este número como argumento a la función isValidCard()

- Función isValidCard()
	si es un campo vacio entonces:
		MOSTRAR un mensaje de error
	si no es un campo vacío entonces:
        Pasar los números a un array en orden inverso
        recorre con un for el largo del nuevo array inverso
            si la posición actual es impar, agregar el dígito a un nuevo arreglo
             si la posición actual es par, multiplicar por dos este dígito
                si el dígito al doble es mayor a diez, sumar sus dos dígitos y agregar este número a su posición en el nuevo arreglo
                si el dígito al doble es menor a diez, agregar este número a su posición en el nuevo arreglo
      recorren con for el largo del array inverso con sus nuevas posiciones y poner la suma de cada dígito en una nueva variable
        si la suma de los dígitos es múltiplo de 10
          mostrar mensaje indicando que la tarjeta es válida
        sino
          mostrar mensaje indicando que la tarjeta no es válida

          
