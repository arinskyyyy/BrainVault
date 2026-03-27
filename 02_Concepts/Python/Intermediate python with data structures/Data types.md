
fundamental data types :

i) int - integer
ii) float - decimal
iii) str - sequence of characters
iv) bool - True or False

What is data structures?
--
It is a structure/ containers that let us organize and store the data effectively and allows to manipulate the data.

Python data structures contains :

i) list [ brackets ] - mutable
- stores different type of items in order. 
- nested list : list inside list, example : [1, 2, 3, 4, [5, 6, 7, 8]]

ii) tuples ( parenthesis ) - immutable
- cannot be changed after creation
- usage : require to store something permanently
- example : ('Hmm',) or 'Greetings',
- -list, tuple : accessible by index

iii) dictionaries { braces } - access and stores using key : value pairs
- accessible by keys
- keys must be unique and immutable
- example : dic = {'size' : 6, 'rounds' : 4, 'speed' : 2, 'pressure' : 'fast'} | print(dic['size'])
- dictionaries methods : .keys( ) returns all the keys, .values( ) returns all the values, .items( ) returns all of the items (both keys and values)

iv) sets { braces } or set( ) - 
- unique items, no duplicates
- unordered
- example : set_example = {val3, val1, val2}
- set methods : .union( ) combines or combine using | , .intersection( ) commons &,
- .difference( ) - :
    - set1 = {1, 2, 3, 4} set2 = {3, 4, 5, 6} 
    - difference_result = set1.difference(set2)
    - output : {1, 2}
- .add( ), .remove( ), by element, not index

