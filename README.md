# python-assignment-5
# Python Basic Assignment - 5
# 1. What does an empty dictionary's code look like?
# Empty dictionary
emptyDict = {}
type(emptyDict)

# 2. What is the value of a dictionary value with the key 'foo' and the value 42?
# The value will be 42
my_dict = {'foo': 42}
my_dict['foo']

# 3. What is the most significant distinction between a dictionary and a list?
# The dictionary is created using {} or dict()
dict3 = {'k1': 123, 'k2': 2+3j}

# The list is created using [] or list()
list3 = [12,23,45]

# 4. What happens if you try to access spam['foo'] if spam is {'bar': 100}?
# It will throw an error

spam = {'bar': 100}
spam['foo']

# 5. If a dictionary is stored in spam, 
# what is the difference between the expressions 'cat' in spam and 'cat' in spam.keys()?
# There is no difference
# 'cat' in spam: This expression checks whether there is a 'cat' KEY in the dictionary
# 'cat' in spam.keys(): This will checks whether there is a key 'cat' in spam.

dict5 = {'k1': 123, 'k2': 2+3j}
a = 'k1' in dict5
b = 'k1' in dict5.keys()
print(a, b)

# 6. If a dictionary is stored in spam,
# what is the difference between the expressions 'cat' in spam and 'cat' in spam.values()?

# Difference:
# 'cat' in spam: This expression checks whether there is a 'cat' KEY in the dictionary
# 'cat' in spam.values(): This will checks whether there is a value 'cat' in spam.

spam = {'cat': 123, 'k2': 2+3j}
a = 'cat' in spam
b = 'cat' in spam.values()
print(a, b)

# 7. What is a shortcut for the following code?
# if 'color' not in spam:
# spam['color'] = 'black'

spam
# shortcut code 
spam.setdefault('color', 'black')
spam

# 8. How do you "pretty print" dictionary values using which module and function?
# By importing pprint and using pprint.pprint(dict_name)

import pprint
pprint.pprint(spam)
