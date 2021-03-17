# Assignment4
hat exactly is []? Answer :- These are parenthesis are used to specify the subscript in lists , array etc.
In [ ]:
2. In a list of values stored in a variable called spam, how would you assign the value 'hello' as the third value? (Assume [2, 4, 6, 8, 10] are in spam.)
In [5]:
spam=[2, 4, 6, 8, 10]
In [6]:
spam[2]='hello'
In [7]:
spam
Out[7]:
[2, 4, 'hello', 8, 10]
In [ ]:
3. What is the value of spam[int(int('3' * 2) / 11)]?
In [8]:
spam=['a', 'b', 'c', 'd']
In [9]:
spam[int(int('3' * 2) / 11)]
Out[9]:
'd'
In [ ]:
4. What is the value of spam[-1]?
In [10]:
spam[-1]
Out[10]:
'd'
In [12]:
spam[:2]
Out[12]:
['a', 'b']
In [21]:
bacon=[3.14, 'cat', 11, 'cat', True]
In [22]:
bacon.index('cat')
Out[22]:
1
In [24]:
bacon.append(99)
In [25]:
bacon
Out[25]:
[3.14, 'cat', 11, 'cat', True, 99]
In [26]:
bacon.remove('cat')
In [27]:
bacon
Out[27]:
[3.14, 11, 'cat', True, 99]
What are the list concatenation and list replication operators?

In [1]:
list=[1,2,3,4]
In [2]:
list+[5]  //concatenation
Out[2]:
[1, 2, 3, 4, 5]
In [3]:
list*2    //replication
Out[3]:
[1, 2, 3, 4, 1, 2, 3, 4]
What is difference between the list methods append() and insert()?
In [4]:
list.append(10)
In [5]:
list
Out[5]:
[1, 2, 3, 4, 10]
In [7]:
list.insert(3,55)
In [8]:
list
Out[8]:
[1, 2, 3, 55, 4, 10]
What are the two methods for removing items from a list?

In [9]:
list=[1,2,3,4,5,6,7,8,9]
In [10]:
list.pop(7)//method 1
Out[10]:
8
In [11]:
list
Out[11]:
[1, 2, 3, 4, 5, 6, 7, 9]
In [12]:
list.remove(4)//method 2
In [13]:
list
Out[13]:
[1, 2, 3, 5, 6, 7, 9]
Describe how list values and string values are identical.

answer :-both are ordered collection of data

In [ ]:
Whats the difference between tuples and lists?
In [14]:
tuple_=("morning","afternoon","evening","night")
List_=["morning","afternoon","evening","night"]
In [15]:
List_[2] = 5
print(List_)

tuple_[2] = 5
['morning', 'afternoon', 5, 'night']
---------------------------------------------------------------------------
TypeError                                 Traceback (most recent call last)
<ipython-input-15-f7405ee94773> in <module>
      2 print(List_)
      3 
----> 4 tuple_[2] = 5

TypeError: 'tuple' object does not support item assignment
How do you type a tuple value that only contains the integer 42?
In [20]:
tuple_=(42,)
In [21]:
type(tuple_)
Out[21]:
tuple
How do you get a list value's tuple form? How do you get a tuple value's list form?
In [22]:
list_=[10,20,30,40,50]
tuple_=(10,20,30,40,50)
In [23]:
type(list_)
Out[23]:
list
In [24]:
type(tuple_)
Out[24]:
tuple
In [25]:
type(tuple(list_))
Out[25]:
tuple
In [29]:
list(tuple_)
---------------------------------------------------------------------------
TypeError                                 Traceback (most recent call last)
<ipython-input-29-96e7e5e9b194> in <module>
----> 1 list(tuple_)

TypeError: 'list' object is not callable
Variables that "contain" list values don't actually contain lists directly. What do they contain instead?

they will contaion reference of the list

How do you distinguish between copy.copy() and copy.deepcopy()?

In [31]:
import copy  
li1 = [1, 2, [3,5], 4]    
li2 = copy.copy(li1)  
li3 = copy.deepcopy(li1)
In [32]:
li2
Out[32]:
[1, 2, [3, 5], 4]
In [33]:
li3
Out[33]:
[1, 2, [3, 5], 4]
