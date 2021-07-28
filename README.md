# Python

# 😎 Day 1

## Working with Variables in python to manage data

- Day1 Stuff
    - ✅ Course Pledge
    - Tips for Taking the Course
        - [ ]  Use another Screen
        - [ ]  Python syntax Cheat sheet
        - [ ]  Keeping the motivation High [link](https://www.udemy.com/course/100-days-of-code/learn/lecture/23518346#search)
        - [ ]  Note down how the code works while yout mind is fresh

    ---

    # Summary

    - [x]  Printing
    - [x]  Commenting
    - [x]  Debugging
    - [x]  String Manipulation
    - [x]  Variables

    ---

    ## Printing

    ```python
    print("hello wolrd"); 
    print('hello wolrd'); #Does not matter wheter the quotes are single or twice
    ```

    ## Commenting

    ```python
    # This is a comment yay
    ```

    ## Debugging

    - Pay attention to the color highlinig

    ## String Manipulation

    ```python
    print("hello wolrd \n alo"); 
    # \n allows us to jump line
    #----
    #Concatenate strings
    print("hello" + " " + "Daniel"); 
    ```

    ## Input function

    ```python
    input("promp -> what the user see"); 
    # we can nest it
    print("Hello " + input("what is your name?")); 
    # when I run it: first it will display the input and then wait for the user 
    # response, then finally it will display the print with the variable

    ```

    ![Python%20003f99b560234cc5b475d85d47d3d2f3/Screen_Shot_2021-07-18_at_6.45.01_PM.png](Python%20003f99b560234cc5b475d85d47d3d2f3/Screen_Shot_2021-07-18_at_6.45.01_PM.png)

    ## Print the number of characters given a string

    ### len()

    ```python
    #len() -> fucntion which return the length of the given paramether
    print(
    	len(
    		input("your name")
    	)
    ); 
    ```

    ## Variables

    ```python
    name = input("What is your name");
    print(name); 
    ```

---

# 👍 Day 2

## Understanding data types and how to manipulate strings

- Day2 Stuff
    - [x]  Data Types
        - [x]  type()
        - [x]  str()
        - [x]  float()
    - [ ]  Mathematical operations

    ---

    # Python Data Types

    - Types

        ## String

        - "Hello"
        - Character → "Hello"[0]
            - Pulling out a particular element from a string is called: Subscripting

        ## Integer

        - 1231 +21321
        - Large Integers
            - 123_123_123 → same as → 123123123

        ## Float

        - Floating-point number
        - 3.14159

        ## Boolean

        - True → Capital T
        - False → Capital F

        ---

        # Type checking

        ```python
        print(type(123)) #int
        ```

        # Type conversion (casting)

        ```python
        # to String
        str(12324)

        # to Float
        float("12.3")
        ```

    ---

    # Mathematical operations

    - Math

        ```python
        1+2
        1-2
        3*3
        3/1 # always ends up with floating number even if the result is not decimal
        2**2 # Exponents -> rise a number to a power 
        ```

        ## Rule: PEMDAS

        - P arentheses → ()
        - E xponents → **
        - M ultiplication → *
        - D ivision → /
        - A ddition → +
        - S ubstraction → -

        Calculations goes left to right

    ---

    # Number manipulation and F strings

    - Numner manipulation

        ```python
        # round a number
        round(8/3)
        # specify the digits of precision you wanna round 
        round(8/3, 2) # 2 digits
        # Floor division
        8//3
        ```

        ## Floor division //

        - We know that whenever we divide any number by other number → the result always gets turned into a floating point number
        - obtener el resultado de una division sin ser float 👍 será int

        ## Modify a value based on the prev value

        ```python
        score = 0; 
        score += 2; 
        score /= 2; 
        .
        .
        .
        ```

        ---

        # F sting

        ```python
        f"string bla bla bla "
        #also
        score = 100; 
        result = f"your score is { score }";
        #Hace por nosotros todas las conversiones yay
        ```

        # Format by given decimal digits

        ### "{:.numf}"

        ### "{:.2f}"

        ### "{:.3f}"

        ```python
        value = "{:.2f}".format(2,454546) # 2.45
        ```

---

# 👀 Day 3

## Control Flow and logical operations

- Day3 Stuff
    - [x]  Conditional statements
    - [x]  Logical operators
    - [x]  Code Blocks
    - [x]  Scope

    ---

    # Conditional statement

    ```python
    if condition:
    	do this
    else:
    	do this
    # ==
    # >
    # <
    # >=
    # <=

    if condition1:
    	do A
    elif condition2:  # elif
    	do B
    else:
    	do C
    ```

    Un bloque de if, elif y else → terminará cuando se cumpla el primero, ignorando a los otros

    # Logical Operators

    ## and

    ```python
    1 > 0 and 1 < 2
    ```

    ## or

    ```python
    3 < 5 or 5 > 9
    ```

    ## not

    ```python
    # es como el !
    not 2 > 1 # false
    not false # true
    ```

    ---

    # "AbCd".lower() → "abdc"

    # "daniel".count("a") → 1

    ---

    # Print more than one line string

    # use ''' → 3 of **'**

    ```python
    print('''
    	_._     _,-'""`-._
         (,-.`._,'(       |\`-/|
             `-.-' \ )-`( , o o)
         -bf-      `-    \`_`"'-
    ''');
    ```

    # use the english symbols inside a string

    ## Use the back slash

    ```python
    print('You\'ve hi "alo" bla bla')
    ```

---

# 👽 Day 4

## Randomisation and Python Lists

- Day4 Stuff
    - [x]  Randomisation
    - [x]  Python Lists

    ---

    - Random

        # 🎲 Randomisation

        - pseudo-random number generators
        - And the one that Python uses is something called the **Mersenne Twister**.

        ```python
        # 1. import it
        import random
        random_integer = random.randint(2,4);  # random num between 2 and 4

        ```

        ## random.randint(a,b) → int random between 2 given ints

        ## random.random() → 0 to 0.999999 (Not includes 1)

        # Random choice

        ```python
        import random
        # given a list of items
        list = [1,2,4,5,6,6,]
        print(random.choice(list)) 
        # it will return a random item from the given list
        ```

        # What is a module in python?

        Basically: parts of code splited up in other files that we can import and use, making our code leaner

        - We can create our own modules → just creating a new file and export it into another file

            ![Python%20003f99b560234cc5b475d85d47d3d2f3/Screen_Shot_2021-07-21_at_4.30.10_PM.png](Python%20003f99b560234cc5b475d85d47d3d2f3/Screen_Shot_2021-07-21_at_4.30.10_PM.png)

            ![Python%20003f99b560234cc5b475d85d47d3d2f3/Screen_Shot_2021-07-21_at_4.30.33_PM.png](Python%20003f99b560234cc5b475d85d47d3d2f3/Screen_Shot_2021-07-21_at_4.30.33_PM.png)

    - Lists

        # Python Lists

        The list is what you would call a data structure.

        - it's just a way of organizing and storing data in Python.
        - list = [item1, item2]

        You can also use negative numbers [-1] So if I wrote -1 or -2, then it actually starts counting from the end of the list.

        ## Add elements to the list:

        ```python
        list.append("newi_tem")
        ```

        ## Remove elements from the list:

        ```python
        list.remove(index) 
        ```

        ## Add a bunch of elements

        ```python
        list.extend(["elem1", "elem2", "elem3" ...])
        ```

        ## Remove all the items of the list

        ```python
        list.clear()
        ```

        ---

        # Split → same as JS

        - Works the same as JS yay

        ```python
        "daniel, daniel, ".split(", ")
        ```

        # Sum all the items of an array

        ```python
        list = [1,2,3,4]
        result = sum()
        ```

        # Max number in a list

        ```python
        list = [1,2,3,4,5]
        max(list) #5
        ```

        # Shuffle a list

        ```python
        import random
        x = [1,2,3,4,5]
        random.shuffle(x)
        ```

        # Check if a elment is in a list

        ```jsx
        listA = ['Stranger Things', 'S Education', 'Game of Thrones']

        if 'S Eductation' in listA:
            print("Yes, 'S Eductation' found in List : ", listA)
        ```

        # List comprehension

        ```python
        # example
        fruits = ["apple", "banana", "cherry", "kiwi", "mango"]
        newlist = []
        for x in fruits:
          if "a" in x:
            newlist.append(x)

        #with List comprehension -------------------------

        fruits = ["apple", "banana", "cherry", "kiwi", "mango"]
        newlist = [x for x in fruits if "a" in x]
        ```

---

# 💣 Day 5

## Python Loops

- Day5 stuff

    # Loops

    ## For Loop

    ```python
    for item in list:
    	#Do something to each item
    ```

    ## For range

    ```python
    for n in range(a,b, step #optional step):
      print(n)
    #0
    #1
    #2
    #3
    #4
    ```

---

# 💪🏻 Day 6

## Functions, Code Blocks and While Loops

- Day6 stuff
    - Functions

        # Functions

        - Create our own functions

        ```python
        def name():
        	print("hello")

        name()
        ```

        - 
    - While loop

        # While Loop

        ```python
        condition = 6
        while condition > 0:
        	#Do something
        	condition -= 1 
        ```

        # When use For Loop or While Loop

        for loops are really great when you want to iterate over something and you need to do something with each thing that you are iterating over.                               while loop when you don't really care what number in a sequence you're in, which item you're iterating through in a list and you just simply want to **carry out some sort of functionality many, many times until some sort of condition that you set.**

---

# ✅ Day 7

## Hangman Project

- Day7 stuff

    # Import files

    ```python
    form file import cosa1, cosa2
    ```

    # Clear

    ```python
    from replit import clear
    clear()
    ```

---

# 🥴 Day 8

## Functions with Inputs

- Day8 stuff
    - [x]  Functions with inputs
    - [x]  Difference between Arguments and Parameters

    ---

    # Functions and inputs

    ```python
    def my_func(param):
    	#Something
    	print(param)

    my_func("hello")
    ```

    ![Python%20003f99b560234cc5b475d85d47d3d2f3/Screen_Shot_2021-07-26_at_9.52.38_AM.png](Python%20003f99b560234cc5b475d85d47d3d2f3/Screen_Shot_2021-07-26_at_9.52.38_AM.png)

    The parameter is the name of the data that's being passed in,

    the argument is the actual value of the data

    # Positional vs Keyword arguments

    ```python
    #Positional
    def my_positional(a,b,c):
    	print(f"{a}, {b}, {c}")

    my_positional(3,2,1) # a = 3, b = 2, c = 1
    my_positional(1,2,3) # a = 1, b = 2, c = 3. the order matters

    #Keyword

    def my_keyword(a,b,c):
    	print(f"{a}, {b}, {c}")

    my_keyword(a=1,b=2,c=3) #No matters the order
    my_keyword(c=3,b=2,a=1)
    	

    ```

    ## Check wether a number is prime

    ```python
    def prime_checker(number):
      is_prime = True
      for num in range(2,number):
        if number % num == 0:
          is_prime = False
      if is_prime:
        print("It's a prime number.")
      else:
        print("It's not a prime number.")
    ```

---

# ⛹️‍♂️ Day 9

## Dictionaries & Nesting

- Day9 stuff
    - [x]  Dictionaries
    - [x]  Nesting

    ---

    - Dictionary

        # Dictionaries

        - key and value

            ![Python%20003f99b560234cc5b475d85d47d3d2f3/Screen_Shot_2021-07-26_at_12.46.36_PM.png](Python%20003f99b560234cc5b475d85d47d3d2f3/Screen_Shot_2021-07-26_at_12.46.36_PM.png)

            ```python
            # declarar
            my_dictionary = {
            	"key":"value",
            	"key2":"value2"
            	123: "value3" #valid
            	abc: "cc" #invalid 
            }
            # acceder
            my_dictionary["key2"]

            #add value
            my_dictionary["key4"] = "nueva data "

            # create an empty dictionary
            empty_one = {}

            #Wipe an existing dictionary
            my_dictionary = {} # like clear
            ```

            ## Iterate a dictionary

            ```python
            my_dictionary =  {
            	"a" : 1
            	"b" : 2
            	"c" : 3
            }
            for key in my_dictionary: 
            	print(key)
            # a
            # b
            # c

            # ----

            for key in my_dictionary: 
            	print(my_dictionary[key])
            ```

    - Nesting

        # Nesting

        ```python
        my_test = {
        	"list" : [1, 2, 3, 4, 5],
        	"dic" : {
        		"elem" : 1,
        	}
        }
        ```

---

# 🐙 Day 10

## Functions with Outputs

- Day10 stuff

    # Functions with Output

    and these are functions which allow you to have an output once the function is completed.

    ```python
    def my_funct():
    	result = 3 * 2
    	return result # pretty much like JS

    my_result = my_func() #6

    ```

    ## Convert an string to Title form python

    ```python
    ''.join(x for x in 'my title'.title() if not x.isspace())

    #MyTitle
    ```

    ## Return as a way to scape a function

    ```python
    def format_name(f_name, l_name):
    	if f_name == "" or l_name == "":
    		return ## then, everithing bellow will be ignored

    	
    ```

    ---

    # Docstrings in python

    - Documentation of functions → which explains the function expected behaviour

    ```python
    # The docstring has to go as the first line after the declaration.
    # and then after the colon, the first indented line will be the docstring.
    # use 3 of "
    def my_func():
    	"""Bla bla bla documentation bla bla"""
    	# function stuff uwu
    	
    ```

    - it would look like

        ![Python%20003f99b560234cc5b475d85d47d3d2f3/Screen_Shot_2021-07-27_at_8.25.01_PM.png](Python%20003f99b560234cc5b475d85d47d3d2f3/Screen_Shot_2021-07-27_at_8.25.01_PM.png)