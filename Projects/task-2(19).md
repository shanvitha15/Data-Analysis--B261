### 1) - a) 

#### Document today’s class with proper explanation using markdown, comments, examples and code.

### 1) - b)

#### Use help() to understand each parameter of all the string methods that were covered in class so far.

 ### 1) String_find() :
 
 * string find operation refers to searching for a specific sequence of characters (a substring) within a larger text or string.
 
 * When you use string find, to an program or to computer program to check if a particular set of characters exists within a given text, and it will return a result that tells you whether or where that substring was found.
 
 * it's found, the program may tell you the position (index) where it starts in the text.
 
 ### Syntax of str.find() :

 
        S.find(sub[, start[, end]])
   
    where,
   
 * sub : sub-string
 * start : from the starting of index position
 * end : till upto the index position
 * returns the lowest index in a S where a sub-string is found in the format of <b>S[start:end]</b>.
 * return <b>-1</b> on failure.
 


```python
x = '''Peter Piper picked a peck of pickled peppers.
A peck of pickled peppers Peter Piper picked.
If Peter Piper picked a peck of pickled peppers,
Where’s the peck of pickled peppers Peter Piper picked'''
x
```




    'Peter Piper picked a peck of pickled peppers.\nA peck of pickled peppers Peter Piper picked.\nIf Peter Piper picked a peck of pickled peppers,\nWhere’s the peck of pickled peppers Peter Piper picked'




```python
x.find('a',20)
```




    114




```python
x.find('z',120)
```




    -1



### 2) String _rfind() :

*  string rfind refers to the operation of searching for a specific sequence of characters (substring) within a larger text or string, but it starts the search from the end of the string and works backward.

* When you use string find, to an program or to computer program to check the last occurrence of a particular set of characters in a given text and report its position (index) within the text.

* If the substring is found multiple times, it will return the position of the last occurrence.

#### Syntax of string_rfind() :


        S.rfind(sub[, start[, end]])
      
     where,
    
 * sub : sub-string
 * start : from the starting of index position
 * end : till upto the index position  
 * Return the highest index in S where substring sub is found,
    such that sub is contained within <b>S[start:end]</b>.  
 * Return <b>-1</b> on failure.


```python
'malayalam'.rfind('a',2)
```




    7




```python
'malayalam'.rfind('z',10)
```




    -1



<b> the main difference between the find and rfind as following :
    
1. find - moves from left to right, and retruns the lowest index in the given string
2. rfind - moves from right to left, and retruns the highest index in the given string </b>

 ### 3) String_Count () :
 
 * string count refers to the operation of counting how many times a specific substring appears within a larger text or string.
 
 * When you use string count, to an program or to computer program to check for a certain sequence of characters within a given text and then return the number of times that sequence is found.
 
### Syntax of str.count () :

<b>S.count(sub[, start[, end]])</b>

     where,
     
 * sub : sub-string
 * start : from the starting of index position
 * end : till upto the index position
 * Return the number of non-overlapping occurrences of substring sub in
    string <b>S[start:end]</b>.
 * return <b>0</b> on failure.
 


```python
x
```




    'Peter Piper picked a peck of pickled peppers.\nA peck of pickled peppers Peter Piper picked.\nIf Peter Piper picked a peck of pickled peppers,\nWhere’s the peck of pickled peppers Peter Piper picked'




```python
x.count('p')
```




    28




```python
x.count('z')
```




    0



 ### 4) String_Index() :
 
 * string index refers to the position of a specific character within a text or string.
 * Each character in a string is assigned a unique index number that represents its position within the string from beginning. 
 * index numbers typically start at 0 for the first character in the string and increase incrementally for each subsequent character.
 
 #### syntax for str.index() :
 
          S.index(sub[, start[, end]])
      
     where,
* sub : sub-string
* start : from the starting of index position
* end : till upto the index position     
* Return the lowest index in S where substring sub is found,such that sub is contained within <b>S[start:end]</b>
*  Raises <b>ValueError</b> when the substring is not found.


```python
z = 'kanada'
z.index('k')
```




    0




```python
z = 'kanada'
z.index('z')
```


    ---------------------------------------------------------------------------

    ValueError                                Traceback (most recent call last)

    <ipython-input-12-6b9b28265771> in <module>
          1 z = 'kanada'
    ----> 2 z.index('z')
    

    ValueError: substring not found


<b>the difference between the find(), and index() is </b>:
 * in find() if we dont have any variable doesnt have in that string is gives -1 in output.
 * but in index(), it shows an error so that we can't run the program.

### 5) String_rindex() :

* string rindex refers to finding the position (index) of a specific character or substring within a text or string.
* but it starts the search from the end of the string and works backward,and moving towards the beginning.

#### Syntax for str.rindex() :
     
     S.rindex(sub[, start[, end]])
    
    where,
* sub : sub-string
* start : from the starting of index position
* end : till upto the index position
* Return the highest index in S where substring sub is found,
    such that sub is contained within <b>S[start:end]</b>.
* Raises <b>ValueError</b> when the substring is not found.

### index() and rindex() are same but :
* index () - from left to right begins with index = 0(lowest index)
* rindex () - from right to left befins with index = n(highest index)


```python
z = 'kanada'
z.index('n')
```




    2




```python
z = 'kanada'
z.index('y')
```


    ---------------------------------------------------------------------------

    ValueError                                Traceback (most recent call last)

    <ipython-input-14-068493ee89fd> in <module>
          1 z = 'kanada'
    ----> 2 z.index('y')
    

    ValueError: substring not found


### 6) String_Replace () :

* string replace refers to the operation of changing one set of characters (substring) within a text or string to another set of characters.
* editing or modifying a piece of text by replacing specific words, phrases, or characters with different ones.

#### syntax for str.replace() :

     replace(old, new, count=-1, /)
     
    where,
    
* old : the old sub-string
* new : the new sub-string
* count : how many times we have to change the old string to new string <b>defalut value = -1</b>
* '/' : new line



```python
m='malayalam'
m.replace('m','M')
```




    'MalayalaM'




```python
m.replace('a','A',2) # count value = increse to 2
```




    'mAlAyalam'




```python
m.replace('a','A',4) # count value = increse to 4
```




    'mAlAyAlAm'



### 7) String_Split() :

* string split refers to the operation of dividing a longer piece of text or string into smaller parts based on a specific character or sequence of characters. 
* like breaking a sentence into individual words or splitting a paragraph into sentences.
* When you use string count, to an program to find a specific character, such as a space or a comma, within the text and use that character as a delimiter to separate the text into smaller pieces, often resulting in an array or a list of substrings.

#### syntax for str.split() :

       split(sep=None, maxsplit=-1)
       
      where,
* None : the default value(white space)
* maxsplit : we can increase the maxsplit value upto our choice.
* defalut value <b>-1 </b>


```python
x = 'Innomatics Research Labs, near JNTU'
x.split(' ')
```




    ['Innomatics', 'Research', 'Labs,', 'near', 'JNTU']




```python
x = '''Betty Botter bought some butter
But she said the butter’s bitter
If I put it in my batter, it will make my batter bitter
But a bit of better butter will make my batter better
So ‘twas better Betty Botter bought a bit of better butter'''
x.split(' ', maxsplit = 4) # left to right
```




    ['Betty',
     'Botter',
     'bought',
     'some',
     'butter\nBut she said the butter’s bitter\nIf I put it in my batter, it will make my batter bitter\nBut a bit of better butter will make my batter better\nSo ‘twas better Betty Botter bought a bit of better butter']



### 8) String_rsplit() :

* string rsplit is similar to string split, but it splits a longer piece of text or string into smaller parts based on a specific character or sequence of characters starting from the end of the string and working <b>backward</b>.
* breaking a sentence into individual words starting from the <b>last word and moving towards the beginning</b>.

#### syntax for str.rsplit() :
   
      x.rsplit(sep=None, maxsplit=-1)
      
    where,
    
* sep : The delimiter according which to split the string default : <b> none</b>
* maxsplit : Maximum number of splits to do defalut : <b>-1</b> 


```python
x.rsplit(' ',maxsplit = 5) #right to left
```




    ['Betty Botter bought some butter\nBut she said the butter’s bitter\nIf I put it in my batter, it will make my batter bitter\nBut a bit of better butter will make my batter better\nSo ‘twas better Betty Botter bought',
     'a',
     'bit',
     'of',
     'better',
     'butter']



### 10) String_Partition () :

* string partition refers to the operation of splitting a longer piece of text or string into three parts based on a specific separator or delimiter. 
* It's like dividing a sentence into three segments around a particular word or character.

      The operation will result in three components:

         * The part of the string before the separator.
         * The separator itself.
         * The part of the string after the separator.

#### syntax for str.partition() :

         partition(self, sep, /)
         
      where,  
* Partition the string into three parts using the given separator.
* If the separator is not found, returns a 3-tuple containing the original string.
* two empty strings.




```python
x.partition(' ') 
```




    ('Betty',
     ' ',
     'Botter bought some butter\nBut she said the butter’s bitter\nIf I put it in my batter, it will make my batter bitter\nBut a bit of better butter will make my batter better\nSo ‘twas better Betty Botter bought a bit of better butter')




```python
x.partition('z')
```




    ('Betty Botter bought some butter\nBut she said the butter’s bitter\nIf I put it in my batter, it will make my batter bitter\nBut a bit of better butter will make my batter better\nSo ‘twas better Betty Botter bought a bit of better butter',
     '',
     '')



### String_rpartition () :

* string rpartition is similar to "string partition," but it splits a longer piece of text or string into three parts based on a specific separator or delimiter, <b>starting from the end of the string and working backward</b>. 
*  but the operation begins at the end of the text and moves towards the beginning.

        The operation results in three components:
      * The part of the string after the last occurrence of the separator.
      * The separator itself.
      * The part of the string before the last occurrence of the separator.
      
   #### syntax for str.rpartition () :
   
           rpartition(self, sep, /) 
           
         where,
         
      * the separator is found, returns a 3-tuple 
      * the separator is not found, returns a 3-tuple containing two empty strings and the original string.


```python
m = 'monkey'
m.rpartition('o') # left to right - direction
```




    ('m', 'o', 'nkey')




```python
m = 'monkey'
m.rpartition('a') # right to left - direction
```




    ('', '', 'monkey')



### String_SplitLines () :

* string splitlines refers to the operation of splitting a text or string into multiple lines based on line breaks or newline characters. 
* program to find and identify the newline characters within the text,hese lines are usually stored as elements in a list or array.  

 #### syntax for str.splitlines() :
 
      splitlines(self, /, keepends=False)
      
    where,
    
  * Return a list of the lines in the string, breaking at line boundaries.
  * Line breaks are not included in the resulting list unless keepends is given and true.
    


```python
x.splitlines()
```




    ['Betty Botter bought some butter',
     'But she said the butter’s bitter',
     'If I put it in my batter, it will make my batter bitter',
     'But a bit of better butter will make my batter better',
     'So ‘twas better Betty Botter bought a bit of better butter']


