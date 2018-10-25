
---------------------------------------
# LISTS
---------------------------------------

-------------
## Exercise 1

### PART 1

Fill in the blanks so that the program below produces the output shown.

```
values = ____
values.____(1)
values.____(3)
values.____(5)
print('first time:', values)
values = values[____]
print('second time:', values)
```

#### Output:
first time: [1, 3, 5]
second time: [3, 5]

### PART 2

Fill in the blanks so that the program below produces the output shown.

```
values = [1]
values.____(____)
print('first time:', values)
values._____()
print('second time:', values)
```

#### Output:
```
first time: [1, 3, 5]
second time: [3, 5]
```

-------------
## Exercise 2

```
numbers = [3, 5, 8, 2, 4, 9, 0]
```

#### Output:
```
[0, 2, 3, 4, 5, 8, 9]
```

Look into the set of list methods to sort the items in the numbers list.


-------------
## Exercise 3 - optional


Given this:

```
print('string to list:', list('tin'))
print('list to string:', ''.join(['g', 'o', 'l', 'd']))
```

#### Output:
```
['t', 'i', 'n']
'gold'
```

* Explain in simple terms what list('some string') does.
* What does '-'.join(['x', 'y']) generate?


-------------
## Exercise 4

```
element = list('helium')
print(element[-1])
```

How can you display all elements but the last one without changing the variable? (Hint: use a combination of slicing and negative indexing.)


-------------
## Exercise 5

```
element = [0, 1, 2, 3, 4, 5, 6, 7, 8]
```

What expression would select all of the even-numbered items from the collection `element`?


---------------------------------------
# FOR loops
---------------------------------------

-------------
## Exercise 1

Fill in the blanks in the program below so that it prints “nit” (the reverse of the original character string “tin”):

```
original = "tin"
result = ____
for char in original:
    result = ____
print(result)
```

-------------
## Exercise 2


Fill in the blanks in each of the programs below to produce the indicated result.

```
# Total length of the strings in the list: ["red", "green", "blue"] => 12
total = 0
for word in ["red", "green", "blue"]:
    ____ = ____ + len(word)
print(total)
```

```
# List of word lengths: ["red", "green", "blue"] => [3, 5, 4]
lengths = ____
for word in ["red", "green", "blue"]:
    lengths.____(____)
print(lengths)
```

```
# Concatenate all words: ["red", "green", "blue"] => "redgreenblue"
words = ["red", "green", "blue"]
result = ____
for ____ in ____:
    ____
print(result)
```

-------------
## Exercise 3

Reorder and properly indent the lines of code below so that they print an array with the cumulative sum of data. The result should be [1, 3, 5, 10].

```
cumulative += [sum]
for number in data:
cumulative = []
sum += number
sum = 0
print(cumulative)
data = [1,2,2,5]
```

---------------------------------------
# Looping data sets
---------------------------------------

-------------
## Exercise 1


Which of these files is not matched by the expression `glob.glob('data/*as*.csv')`?


- data/gapminder_gdp_africa.csv
- data/gapminder_gdp_americas.csv
- data/gapminder_gdp_asia.csv


-------------
## Exercise 2

Modify this program so that it prints the number of records in the file that has the fewest records.

```
import glob
import pandas
fewest = ____
for filename in glob.glob('data/*.csv'):
    dataframe = pandas.____(filename)
    fewest = min(____, dataframe.shape[0])
print('smallest file has', fewest, 'records')
```

Notice that the shape method returns a tuple with the number of rows and columns of the data frame.

(+ optional extend to get the filename itself as well)












