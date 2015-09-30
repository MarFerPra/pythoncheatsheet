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
len(cadena) # número de caracteres
print(cadena)
cadena.find("panic")  # devuelve el indice del comienzo de la cadena buscada, -1 en caso de no encontrarla.
cadena = cadena.replace("Don't", "You should") # substitución del primer argumento por el segundo.



