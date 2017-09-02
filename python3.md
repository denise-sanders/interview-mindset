Pythonic quick ref guide.

## Comprehensions
### List Comprehension
["Kumquats" for x in range(5)] -> ["Kumquats", "Kumquats", "Kumquats", "Kumquats", "Kumquats"]
["Kumquats" for x in range(5) if x < 3] -> ["Kumquats", "Kumquats", "Kumquats"]
### Set Comprehension
{"Kumquats" for x in range(5)} -> {"Kumquats"}
### Dict Comprehesion
{x:False for x in range(3)} -> {0: False, 1: False, 2: False}
### Generator
(x ** 2 for x in range(100)) -> Iterable, generator object that can be converted to an iterable container (like a list) or be a paramter to a function that takes an interable (like sum).
^It's a lazy evaluation thing, great for performance when you do not need a while list/set/whatever of your data. Its an iterable you are consuming.

## Built ins
### Type ones:
ascii, bin (converts integer to binary), bool, bytearray (mutable), bytes (immutable), chr, ord, complex, float, hex, oct, 
### Math ones:
abs, min, max, pow, range, sum, round <- if number ends in .5, it is rounded toward even choice (whyyyyy)
### Meta 
callable, delattr, dir, getattr, globals, hasattr, help, isinatance, issubclass, locals, vars, memoryview, setattr, type
### For the iterables.
Zip returns zip object of elements paired from both lists until one list is consumed
Map(func, iterable) returns map object of result of the func applied to each element in the iterable
Filter(func, iterable) returns filter object of each element in the iterable for which func returns True for

Mutable v Immutable
| Mutable       | Immutable     |
| | |
| set      | frozen-set |
| dict      | there are workarounds |
| lists |   tuple  |
|  |   string  |
| byte array | int, float, long, complex, bytes |