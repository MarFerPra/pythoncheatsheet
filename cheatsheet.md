# Python Cheatsheet

### Depurador

Dentro del código:
```python
import pdb
pdb.set_trace()
```
Fuera del código:
`python -m pdb code.py`

### Profiler

`python -m cProfile code.py`

***

Para pasar de versiones 2.x a 3.x: `script 2to3.py`

***

División real: a/b

División entera: a//b

Valor absoluto: abs(<numero>)

Cambio de base: oct(), bin(), hex()

**Conjuntos**

```python
new_set = set('1234')
new_set = {1,2,3,4}
```

**Cadenas de texto**

```python
new_string = "Cadena de texto"
multiline_string = """Cadena de
texto con multiples
lineas."""

byte_data = b"cadena de tipo byte"
bytearray_data = bytearray("España", "utf16")
```

De 'string' a 'byte': encode()
De 'byte' a 'string': decode()

**Funciones y métodos para strings**

```python
cadena = "Don't panic!"
print(cadena)
len(cadena) # número de caracteres


cadena.find("panic")  # Devuelve el indice del comienzo de la cadena buscada, -1 en caso de no existir.
cadena = cadena.replace("Don't", "You should") # Substitución del primer argumento por el segundo.

cadena.strip() # Elimina espacios en blanco al inicio y al final
cadena.lstrip() # Left strip
cadena.rstrip() # Right strip

cadena.upper() # Paso a mayúsculas
cadena.lower() # Paso a minúsculas
cadena.capitalize() # Inicia la cadena con una mayúscula

cadena = "Life-the universe-and-everything."
cadena.split("-") # Resultado: ['Life','the universe','and','everything.']
cadena.join(",") # Resultado: 'Life,the universe,and,everything.'
```

Concatenación con "+"

Usando '.format()': "This {0} a {1}".format("is","string")

Paso de string a int y viceversa: int(<variable_string>), str(<variable-int>).

Acceso usando índices:
```python
cadena = "01234"
print(cadena[3]) # resultado '3'
print(cadena[:3]) # resultado '012'
```

**Listas**

```python
  lista = [0,1,2,3,4,5]
  lista.append(5) #Añade el elemento al final de la lista. Resultado:  [0,1,2,3,4,5,6]
  lista.insert(2,7) #Añade un elemento en la posición i. Resultado: [0,1,7,2,3,4,5]
  lista.remove(2) #Elimina el primer elemento que tiene el valor que le damos. Resultado: [0,1,3,4,5]
  lista.index(3) #Devuelve el índice del primer elemento que se encuntra con el valor dado. Resultado: 3
  lista.count(3) #Devuelve el número de veces que se repite el valor que se le da. Resultado: 1
  lista.sort() #Ordena la lista, le podemos añadir keys. Resultado: lista, que se encuentra ordenada.
  lista.reverse() #Invierte el orden de la lista. Resultado: [5,4,3,2,1,0]
```
