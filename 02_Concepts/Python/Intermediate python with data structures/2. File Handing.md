
open( ) function - 
- create or open file 
- syntax : file = open('example.txt', 'w') | file = open('filepath', mode)
- modes : how to use the file - 'w' write, 'r' read, 'a' write from the end of a file, 'r+' both read and write
- 'w' overwrites everything in the file, use 'a'.

.write( ) method -
- to write in the file
- syntax : 
-     file.write('This is a line.\n')
-     file.write('This is the next line.\n')

example : 
- with open('diaries.txt', 'w') as file:
    file.write('Date: March 19, 2024 \n')
    file.write('Dear Diary...')

.writelines( ) method -
- write multiple lines.
- syntax : 
-     lines = ['This is a line.\n', 'This is the next line.\n']
-     file.writelines(lines)

.read( ) method -
- syntax : 
-     file = open('filename.txt', 'r')
-     content = file.read()
-     print('Using read():')
-     print(content)

.readlline/s( ) method -
-  lets you read a file one line at a time or multiple lines using readlines

sep and end parameter in print( ) function - 
- both parameters are hidden.
- default value : end='\n', sep=' '
- end : required to modify the ending of print statement.
- sep (separator) : while printing, to differ or modify the distance of values, example :
  [print('item1', 'item2', 'item3', sep='-')]
   output : item1-item2-item3

f-strings -
- formatted string literal.
- example : print(f"I have a total of {apples + bananas} pieces of fruit.")
- calling methods and functions : print(f"You selected: {user_input.capitalize()}")
- round : pi = 3.14159265 print(f"Pi is roughly {pi:.2f}")  # Output: Pi is roughly 3.14
- commas : balance = 1500000 print(f"Your account balance is ${balance:,}") # Output: Your account balance is $1,500,000

.close( ) method -
- to close a file
- example : file.close()

with block - 
- no .close( ) method necessary
- example : with open('filepath', 'mode') as f: