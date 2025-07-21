**JHONATAN-DAVID-PINTO-ANDRADE J3**

# TALLER GUIADO CARACTERES EN PYTHON

## EJERCICIO 1

```python
# Primero usamos "input" para solicitar al usuario que ingrese una frase:
frase = input("Escribe una frase: ")

# "len" es para contar cuantos caracteres tiene dicha frase y los almacena en la variable "total_caracteres":
total_caracteres = len(frase)

# "count" busca cuántas veces aparece el carácter espacio en la frase y lo almacena en la variable "espacios":
espacios = frase.count(" ")

# "print" es para mostar cosas en pantalla, aca le mostramos al usuario cuantos caracteres tiene la frase que ingreso previamente:
print(f"La frase tiene {total_caracteres} caracteres en total.")

# aca le mostramos al usuario cuantos espacios uso en la frase que ingreso previamente:
print(f"La frase tiene {espacios} espacios.")
```

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



## EJERCICIO 2

```python
# Solicitamos al usuario que ingrese su nombre completo:
nombre = input("Escribe tu nombre completo: ")

# Con condicional "if" verificamos que el nombre solo tenga letras y comience con mayusculas:
if nombre.replace(" ", "").isalpha():
 
# Ahora revisamos si cada palabra del nombre comienza con mayúscula:
    if nombre.istitle():
        print("El nombre es válido.")
       
# En caso contrario de que no tenga mayusculas le dira al usuario que el nombre debe comenzar con mayusculas:
    else:
        print("El nombre debe comenzar con mayúscula.")
        
# En caso de que el nombre contenga signos o numeros le dira al usuario que el nombre solo debe tener letras:
else:
    print("El nombre solo debe contener letras.")
```

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



## EJERCICIO 3

```python
# Le pedimos al usuario que ingrese una palabra: 
palabra = input("Escribe una palabra: ")

# Invertimos la palabra con "palabra[::-1]":
invertida = palabra[::-1]

# Mostramos el resultado de invertir la palabra al usuario:
print(f"La palabra invertida es: {invertida}")
```

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



## EJERCICIO 4

```python
# Le pedimos al usuario que ingrese una frase:
frase = input("Escribe una frase: ")

# Ciframos la frase y empezamos a remplazar las vocales por "*"
frase_cifrada = frase.replace("a", "*").replace("e", "*").replace("i", "*").replace("o", "*").replace("u", "*")

# Aca hacemos lo mismo pero con las vocales en mayusculas:
frase_cifrada = frase_cifrada.replace("A", "*").replace("E", "*").replace("I", "*").replace("O", "*").replace("U", "*")

# Mostramos al usuario la frase cifrada: 
print(f"La frase cifrada es: {frase_cifrada}")
```

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



## EJERCICIO 5

```python
# Le pedimos al usuario que ingrese una frase:
frase = input("Escribe una frase: ")

# Contamos cuantas veces esta la vocal "a" tanto en minuscula como en mayuscula: 
a = frase.count("a") + frase.count("A")

# Contamos cuantas veces esta la vocal "e" tanto en minuscula como en mayuscula: 
e = frase.count("e") + frase.count("E")

# Contamos cuantas veces esta la vocal "i" tanto en minuscula como en mayuscula: 
i = frase.count("i") + frase.count("I")

# Contamos cuantas veces esta la vocal "o" tanto en minuscula como en mayuscula: 
o = frase.count("o") + frase.count("O")

# Contamos cuantas veces esta la vocal "u" tanto en minuscula como en mayuscula: 
u = frase.count("u") + frase.count("U")

# Sumamos el total de vocales y almacenamos el resultado en la variable "total_vocales":
total_vocales = a + e + i + o + u

# Mostramos el resultado de vocales al usuario:
print(f"La frase tiene {total_vocales} vocales.")
```

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



## EJERCICIO 6

```python
# Le pedimos al usuario que ingrese el numero de telefono: 
telefono = input("Escribe un número de teléfono de 10 dígitos: ")

# Usamos condicional para poder formatear el numero y verificar si tiene 10 digitos y si tiene letras
if len(telefono) == 10 and telefono.isdigit():
    
# Pasamos a encerrar los primeros 3 digitos entre parentesis y separamos el restro a partir del 6 digito con un guion alto "-"    
    telefono_formateado = f"({telefono[:3]}) {telefono[3:6]}-{telefono[6:]}"
    
# Le mostramos al usuario el resultado al formatear el numero: 
    print(f"El número formateado es: {telefono_formateado}")
    
# En caso de que el numero tenga mas de 10 digitos o una letra le mostrara al usuario que el numero debe tener exactamente 10 digitos:
else:
    print("El número debe tener exactamente 10 dígitos.")
```

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



## EJERCICIO 7:

```PY
# Primero pedimos al usuario que ingrese una palabra: 
palabra = input("Escribe una palabra: ").lower()

# Invertimos la palabra: 
invertida = palabra[::-1]

# Si al invertir la palabra, no cambia nada es un palindromo:
if palabra == invertida:
    print("La palabra es un palíndromo.")

# En caso contrario la palabra no es un palindromo:
else:
    print("La palabra no es un palíndromo.")
```

