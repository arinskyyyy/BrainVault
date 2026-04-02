
try and finally -
- try : attempting to run the code
- finally : what happens in the end
     file_path = 'example.txt'
     try:
     file = open(file_path, 'r')
     Perform operations on the file
     finally:
     file.close() # Ensures file close even if an exception occurs
     Reading from a file using read() method
     with open('example.txt', 'r') as file:
     content = file.read()
     print(content)

fiel cursor - 
- .seek( ) method : used to modify or direct the cursor to a specific part/location in a file, example :
     file.seek(10) # move to the 10th byte
- .truncate( ) : limit the file size
     file.truncate(200) # file size limit : 200 bytes
- usefulness : remove or reset content beyond a certain point, trim or extend the file size as needed

