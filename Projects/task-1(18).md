### 1)
### a)Document today’s class with proper explanation using markdown, comments, examples and code.


## Classes :

* Blue print of the objects.
* defines the properties (attributes) and behaviors (methods) that the objects belonging to that class will have.


```python
print(dir('x'))
```

    ['__add__', '__class__', '__contains__', '__delattr__', '__dir__', '__doc__', '__eq__', '__format__', '__ge__', '__getattribute__', '__getitem__', '__getnewargs__', '__gt__', '__hash__', '__init__', '__init_subclass__', '__iter__', '__le__', '__len__', '__lt__', '__mod__', '__mul__', '__ne__', '__new__', '__reduce__', '__reduce_ex__', '__repr__', '__rmod__', '__rmul__', '__setattr__', '__sizeof__', '__str__', '__subclasshook__', 'capitalize', 'casefold', 'center', 'count', 'encode', 'endswith', 'expandtabs', 'find', 'format', 'format_map', 'index', 'isalnum', 'isalpha', 'isascii', 'isdecimal', 'isdigit', 'isidentifier', 'islower', 'isnumeric', 'isprintable', 'isspace', 'istitle', 'isupper', 'join', 'ljust', 'lower', 'lstrip', 'maketrans', 'partition', 'replace', 'rfind', 'rindex', 'rjust', 'rpartition', 'rsplit', 'rstrip', 'split', 'splitlines', 'startswith', 'strip', 'swapcase', 'title', 'translate', 'upper', 'zfill']
    

# String Methods :
 
* String operations are like tools that you can use to work with text (strings) in computer programming.
* strings are <b>immutable</b>, the resulting strings from string methods have a new memory location.
* in order to use these strings, we need re-assign it to a variable.

### String_Upper_Case():

* This method changes all the characters in a string to capital alphabets.


```python
x = 'hello'
x = x.upper()
x
```




    'HELLO'



#### String_lower_case() :

* This method changes all the characters in a string to small letters.


```python
y = 'PYTHON'
y = y.lower()
y
```




    'python'



###  String_capitalize() :

* This method changes first word, first alphabet will be convert into capital letter.


```python
xc = 'sea shell, see shell, on the sea shore'
xc = xc.capitalize()
xc
```




    'Sea shell, see shell, on the sea shore'



### String_Title() :

* This method changes first alphabet of every word will convert into capital letter.


```python
xt = 'Sea shell, see shell, on the sea shore'
xt = xt.title()
xt
```




    'Sea Shell, See Shell, On The Sea Shore'



### String_Swapcase() :
* This method changes capital letters to small letters and small letters to capital letters. 


```python
xsw = 'Sea Shell, See Shell, On The Sea Shore'
xsw = xsw.swapcase()
xsw
```




    'sEA sHELL, sEE sHELL, oN tHE sEA sHORE'



### String_casefold() :

* This method changes string lower case to more lower case , special characters like Germen character (ß) is already in lower case so, the lower method doesn’t make the conversion.
* but the casefold() method will convert ß to its equivalent character ss


```python
x = 'SjuhdßcnjdGIUN'
x.casefold()
```




    'sjuhdsscnjdgiun'



### 1)
### b) Explain why strings are Immutable by taking a string method as an example. 


* strings are <b>immutable</b>, the resulting strings from string methods have a new memory location.


```python
x = 'abc'
x.upper()
```




    'ABC'




```python
print(id(x), id(x.upper))
```

    1897241356272 1897288544720
    

## 1)
### c) Take a two strings of your choice, 
#### i) Reverse one string

* reversing an string we use indexing operation[start:end:step_size]
* In step size by giving negative value to it, changes the direction from right to left, and it will reversed. 


```python
a = 'innomatics'
b = 'research_Labs'
b = b[::-1]
b
```




    'sbaL_hcraeser'



### ii) Concatenate these two strings

* concatinating two strings, we use <b>+</b> to add these two strings together.


```python
a = 'innomatics'
b = 'research_Labs'
c = a + b
c
```




    'innomaticsresearch_Labs'



### iii) Get the alternate chars of the concatenate string in reverse order.

* first, we take the two strings
* then, we add the strings by using concatination operation and assign these value to new variable
* these variable will reverse the string by using reverse operation, and to get alternative values to that string we use step_size value as <b>-2</b> then we get the required alternate chars of the concatenate string in reverse order.


```python
a = 'innomatics'
b = 'research_Labs'
c = a + b
c = c[::-2]
c
```




    'sa_casrctmni'


