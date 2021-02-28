# **Intermediate Programming Challenges.**


#### **1). pangram**
A pangram is a unique sentence in which every letter of the alphabet is used at least once. The name comes from the Greek root words pan, meaning “all,” and gram, meaning “something written or recorded”.  

### **Problem Description**
The program takes a string and checks if it is a pangram or not. 

### **Algorithm** 
1. Take a string from the user and store it in a variable.
2. Pass the string as an argument to a function.
3. In the function, form two sets- one of all lower case letters and one of the letters in the string.
4. Subtract these both sets and check if it is equal to an empty set.
5. Print the final result.
6. Exit. 

### **Solution**

~~~python 
#python 3.x

from string import ascii_lowercase as asc_lower
def check(s):
    return set(asc_lower) - set(s.lower()) == set([])
strng=input("Enter string:")
if(check(strng)==True):
      print("The string is a pangram")
else:
      print("The string isn't a pangram") 

#python 2.x 

from string import ascii_lowercase as asc_lower
def check(s):
    return set(asc_lower) - set(s.lower()) == set([])
strng=raw_input("Enter string:")
if(check(strng)==True):
      print("The string is a pangram")
else:
      print("The string isn't a pangram")  
~~~ 

### **Solution Explanation** 

1. User must enter a string and store it in a variable.
2. The string is passed as an argument to a function.
3. In the function, two sets are formed- one for all lower case letters and one for the letters in the string.
4. The two sets are subtracted and if it is an empty set, the string is a pangram.
6. The final result is printed.
