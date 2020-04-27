# Python-Size-of-string-in-memory

While working with strings, sometimes, we require to get the size of the string, i.e the length of it. But there can be situations in which we require to get the size that the string takes in bytes usually useful in case one is working with files. Let’s discuss certain ways in which this can be performed.

Method #1 : Using len() + encode()

The simplest and initial method that comes to the mind is to convert the string into a byte format and then extract its size.
# Python3 code to demonstrate 
# getting size of string in bytes 
# using encode() + len() 
  
# initializing string  
test_string = "geekforgeeks"
  
# printing original string  
print("The original string : " + str(test_string)) 
  
# using encode() + len() 
# getting size of string in bytes 
res = len(test_string.encode('utf-8')) 
      
# print result 
print("The length of string in bytes : " + str(res)) 
Output :
The original string : geekforgeeks
The length of string in bytes : 12




Method #2 : Using sys.getsizeof()

This task can also be performed by one of the system calls, offered by Python as in sys function library, the getsizeof function can get us the size in bytes of desired string.

filter_none
edit
play_arrow

brightness_4
# Python3 code to demonstrate 
# getting size of string in bytes 
# using sys.getsizeof() 
import sys 
  
# initializing string  
test_string = "geekforgeeks"
  
# printing original string  
print("The original string : " + str(test_string)) 
  
# using sys.getsizeof() 
# getting size of string in bytes 
res = sys.getsizeof(test_string) 
      
# print result 
print("The length of string in bytes : " + str(res)) 
Output :
The original string : geekforgeeks
The length of string in bytes : 12
