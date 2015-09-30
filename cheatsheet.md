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
