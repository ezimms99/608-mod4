# 608-mod4

Chapter 5 Notes: 

Collections: Prepackaged data structures consisting of related data items. 
Dynamically resize: Growing and shrinking in execution time. 

Lists:
- Lists typically store homogenous data, values of the same data type. 
- Heterogeneous data, data of many different types. 
- Index (an element in a lists, position number) enclosed in [] known as the subscription operator. 
  - First element is indexed as 0
- You can find a lists length using len()
- Lists are mutable - their elements can be modified
- Python's string and tuple sequences are immutable and cannot be modified. 
- Accessing an element that does not exist creates an index error. 
- You can use list elements as variables 
- You can add values to a list using +=
- You can concate two lists, two tuples, or two strings using the +. 
- You can also run comparision operators on multiple lists. 

Tuples: 
- Tuples are immutable and typically store heterogeneous data, but can be homogenous. 
- You can use += to add to a tuple 
- Tuples can contain mutable objects. 

Unpacking Sequences: 
- You can unpack any sequence's elements by assigning the sequence to a comma-separated list of variables. 
- A ValueError occurs if the number of variables to the left of the assignment symbol is not identical to the number of elements in the sequence on the right. 
- You can swap two variables' values using sequence packing and unpacking
- Assessing indices and Values safely with Built-in Function enumerate
  - Preferred mechanism for accessing an element's index and value. 
  - Function recieves an iterable and creates an iterator that, for each element, returns a tuple containing the element's index and value. 
- Creating a Primitive bar chart
  - The for statement uses enumerate to get each element's index and values, then displays a formatted line containing the index, the element value, and the corresponding bar of asterisks. (See Jupyter Notebook). 

Sequence Slicing: 
- Slice sequences to create new sequences of the same type containing subsets of the original elements. 
- The slice copies elements from the starting index to the left of the colon up to, but not including, the ending index to the right of the colon. 
- If you omit the starting index, 0 is assumed. 
- If you omit the ending index, Python assumes the sequence's length. 
- Omitting both the start and end indices copies the entire sequence. 
- You can also use steps to slice, [::2] uses a step of 2 to create a slice of every other number. 
- Using a negative number, slices in reverse order. 
- You can also modify a list by assigning to a slice of it - the rest of the list is unchanged. 
- You can empty an amount of elements as well by using []. 
- You can assign new values by skipping as well. 

Del Statement: 
- The del statement is used to remove elements from a list and delete variables from the interactive session. 
- del listname[-1] gets rid of last element
- del listname[0:2] gets rid of first two elements
- del listname[::2] deletes every other
- del listname[:] removes all.

Passing Lists to Functions: 
- You can create a function that is arbitrary anad then pass a list to it to perform that functions tasks. 
- If you try to pass a tuple to a function it results in a Type Error. 

Sorting Lists:
- Sorting enables you to arrange data either in ascending or descending order. 
- List method sort modifies a list to arrange its elements in ascending order. 
- To order in reverse you use numbers.sort(reverse=True)
- The function sorted returns a new list containing the sorted elements of its argument sequence - the original sequence is unmodified. 
- Tuples and strings do not provide a sort method. 
- Ordering words go in lexicographical order, ie uppercase values will be ordered first. 

Searching Sequences: 
- Searching is the process of locating a key. 
- Index takes as an argument a search key - the value to locate in the list - then searches through the list from index 0 and returns the index of the first element that matches the search key. 
- You can specify the starting and ending indices to search from the starting index up to but not including the ending index location. 
- You can use in to return true or false if a value is in a sequence. 
- Can also use not in to determine if number is not in a sequence. 

Other List Methods:
- Insert adds a new item at a specified index. 
- You can add a new item to the end of a list with method append. 
- List method extend adds all elements of another sequence to the end of a list, equivalent of using +=
- To extend a tuple just use (()) with the tuple values inside -- a type error occurs if you forget the second paranthesis. 
- Remove deletes the first element with a specified value
- To delete all elements use the method clear
- Count searches for its argument and returns the number of times its found. 
- Reverse reverses the contents of a list in place, rather than creating a reversed copy. 
- Copy returns a new list containing a shallow copy of the original list. 

Simulating stacks with lists:
- You push using list method append, which adds a new element to end of list. 
- You pop with no arguments, which repoves and returns the item at the end of the list. 
- First in First out order 
- You will get an index error for pop if the list doesn't contain anything. 

List Comprehensions: 
- A concise and convenient notation for creating new lists. 
- A for clause can iterate to create a list. 
- You can also use aggregate functions to create a list. 
- Can filter elements to select only those that match a condition. 
- Typically produces a list with fewer elements than the data being filtered. 
- You can also process another list and create a new one. 
- A list comprehensions for clause iterates over the specified sequence. 
- A list compregensions if clause filters sequence elements. 

Generator Expressions: 
- Similar to a list comprehension, but creates an iterable generator object that produces values on demand. 
- These are lazy expressions.
- Have to use function list to generate results. 

Filter, Map and Reduce: 
- Use the function filter to obtain odd values in numbers. 
- Functions that recieve other functions as arguments are a functional-style capability called higher-order functions. 
- Can use a lamda rather than a function to define the function inline where it's needed. It's an anonymous function and is by a comma-separated parameter list, a colon and an expression. 
- Function map's first argument is a function that recieves sone value and returns a new value. The second argument is an iterable of values to map. 
- Reductions happen through built-in functions len, sum, min, max. 





