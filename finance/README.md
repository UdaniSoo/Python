# Finance 
### Variables in python
#### Variable names
- Names can be upper or lowser case letters, digots and underscores.
- Varibles can't statrt with a digit
- Some variable names are reserved in pyton.(e.g; class,type) and should be avoided.

#### Variable example
```python 
day_2=5
```

#### Using common way to evaluate stocks

```python 
Price to earning rasio= market Price/ Earning per share
```


Price to earning rasio is a commen way to evaluate stocks. It shows how much investors are willing to pay per dollar earning for stocks.

```python 
price= 200
earning =5
pe_rasio= price/ earning
print(pe_rasio)
```
Python examples
Find the total of revenue_1, revenue_2  revenue_3
```python 
# Print the total revenue
total = revenue_1 + revenue_2 + revenue_3
print(total)

# Print the average revenue
average = total/3
print(average)
```

#### Creating variables
Variables in Python hold a value that may consist of varying data types. Variable names can contain letters, underscores, and numbers.
```python 
revenue_1 = 229.23
print(revenue_1)
```
Output:
```
229.23
```

#### Determining types
Python has a built-in command type() that can determine the type of a variable or literal value.
```python 
# Type of company_1
print(type(company_1))

# Type of year_1
print(type(year_1))

# Type of revenue_1
print(type(revenue_1))
```
Output:
```
<class 'str'>
<class 'int'>
<class 'float'>
```
#### Booleans in Python
Booleans are used to represent True or False statements in Python. Boolean comparisons include:

```python 

>	greater than
>=	greater than or equal
<	less than
<=	less than or equal
==	equal
!=	does not equal
```
E.g: The revenue of company 1 and company 2 are provided as revenue_1 and revenue_2, respectively. Using a comparison operator, determine if revenue_1 is greater than revenue_2.

```python 
# Compare revenue_1 and revenue_2
print(revenue_1 > revenue_2)
```
Output:
```
True
```

#### Combining data types
Different types of data types have different properties. For example, strings and floats cannot be mathematically combined. To convert a variable x to an integer, you can use the command int(x). Similarly, to convert a variable y to a string, you can use the command str(y).

E.g:
- Convert the data type of variables year_1, and revenue_1 to string.
- Use these new variables to create and print the following sentence: "The revenue of Apple in 2017 was $229.23 billion."

```python 
# Update data types
year_1_str = str(year_1)
revenue_1_str = str(revenue_1)
# Create a complete sentence combining only the string data types
sentence = 'The revenue of ' + company_1 + ' in ' + year_1_str + ' was $' + revenue_1_str + ' billion.'

# Print sentence
print(sentence)
```
Output
```
The revenue of Apple in 2017 was $229.23 billion.
```

### Lists in Python

#### Creating lists in Python
A list in Python can contain any number of elements. You generally create a list using square brackets. For example, to create a list of integers, you can use the following command:
```python 
x = [1, 2, 3]
```
E.g:
- Create a list named names containing the strings 'Apple Inc', 'Coca-Cola', and 'Walmart', in that order.
Print names.
- Create a list named prices containing the price of each stock, $159.54, $37.13, and $71.17, in that order.
```python 
# Create and print list names
names = [ 'Apple Inc', 'Coca-Cola', 'Walmart']
print(names[0:])

# Create and print list prices
prices = [159.54, 37.13, 71.17]
print(prices[0:])
```
```
['Apple Inc', 'Coca-Cola', 'Walmart']
[159.54, 37.13, 71.17]
```
#### Indexing list items
Each item in a list has an assigned indexed value. Remember that Python is a zero indexed language, and the first element in a list is stored at index zero. In this exercise, you will practice subsetting single elements from a list.

Q&A
- Print the first element in names.
- Print the second element in names.
- Using a negative index, print the last element in prices.
```python 
# Print the first item in names
print(names)

# Print the second item in names
print(names[1])

# Print the last element in prices
print(prices[-1])
```
```
['Apple Inc', 'Coca-Cola', 'Walmart']
Coca-Cola
71.17
```
#### Slicing multiple list elements

Slicing operations on a list are used to subset multiple elements from a list. The syntax for list slicing is as follows:
```python 
list[start:end]
```
Remember, this syntax indicates subsetting all elements from the start and up to but not including the end element.

Also, you can use extended slicing to efficiently select multiple elements from a list. For example, the following command returns all elements from the list except the first (at index 0):

```python 
x = [1, 2, 3, 4, 5]
x[1:]

[2, 3, 4, 5]
```
Similarly, the following command returns all elements from the list except the last two:
```python 
x[:-2]

[1, 2, 3]
```

Q&A:
Use list slicing to subset the last two elements from names.
```python 
prices = [159.54, 37.13, 71.17]

# Use extended slicing on the list prices
prices_subset = prices[1:]
print(prices_subset)
```

```
[37.13, 71.17]
```

### Lists in Lists

#### Stock up a nested list
Lists can also contain other lists. In the example shown below, x is a nested list consisting of three lists:
```python 
x = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
```
You can use indexing to subset lists within a nested list. To extract the first list within x, you can use the following command:
```python 
x[0]

[1, 2, 3]
```
Q&A
names = ['Apple Inc', 'Coca-Cola', 'Walmart']
prices = [159.54, 37.13, 71.17]

- Create a list named stocks consisting of the lists names and prices, in that order.
- Use list indexing to subset the list prices from stocks (Remember that prices is the second element in stocks).

```python 
# Create and print the nested list stocks
stocks = [['Apple Inc', 'Coca-Cola', 'Walmart'], [159.54, 37.13, 71.17]]
print(stocks)

# Use list indexing to obtain the list of prices
print(stocks[1])
```

### Subset a nested list
You can also extract an element from the list you extracted. To do this, you use two indices. The first index is the position of the list, and the second index is the position of the element within the list.

For example, if you want to extract 7 from x, you can use the following command:
```python 
x = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
x[2][0]

7
```
Here the first index 2 refers to the third list in x and the second index 0 refers to the first element of the third list in x.

Q&A:
stocks = [['Apple Inc', 'Coca-Cola', 'Walmart'], [159.54, 37.13, 71.17]]
1. From the nested list stocks, subset 'Coca-Cola'.
```python 
stocks[0][1]
```
2. From the nested list stocks, subset the price for walmart stock.
```python 
stocks=[1][2]
```

### List methods and functions

#### Exploring list methods and functions
Lists methods and functions are useful for analyses. Functions take objects as inputs or are "passed" an object. Methods, in contrast, act on objects. For lists, useful functions include max() and min(), which identify the maximum or minimum value in a list. A useful list method is .sort() which sorts the elements in a list.

##### Methods Vs. Functions
Methods
- All methods are functions
- List methods are a subset of a built-in functions in python.
- Used on an object
E.g: Price.sort()

Functions
- Not all functions are methods
E.g: type(prices)

Q&A:
1. Using the method .sort(), sort and print the prices in the list prices.
```python 
 Print the sorted list prices
prices = [159.54, 37.13, 71.17]
prices.sort();
print(prices)
```
2. Identify the maximum price in prices using the function max().
```python 
prices = [159.54, 37.13, 71.17]
price_max = max(prices)
print(price_max)
```
```
159.54
```
#### Using list methods to add data
You can use the .append() and .extend() methods to add elements to a list.
##### append()
The .append() method increases the length of the list by one, so if you want to add only one element to the list, you can use this method.

```python 
x = [1, 2, 3]
x.append(4)
x

[1, 2, 3, 4]
```
##### extend()
The .extend() method increases the length of the list by the number of elements that are provided to the method, so if you want to add multiple elements to the list, you can use this method.
```python 
x = [1, 2, 3]
x.extend([4,5,6])
x
[1,2,3,4,5]
```
Q&A
1. Add a single element, 'Amazon.com', to the names.
names = ['Apple Inc', 'Coca-Cola', 'Walmart']
```python 
# Append a name to the list names
names.append('Amazon.com')
print(names)
```
2. Add the list more_elements which consists of two elements to names.

```python 
# Extend list names
more_elements = ['DowDuPont', 'Alphabet Inc']
names.extend(more_elements)
print(names)
```
#### Finding stock with maximum price
Another useful list method is .index(), which returns the index of the element specified. For example, to get the index of 2 in x, you would use:
```python 
x = [1, 2, 3, 4]
x.index(2)

1
```
You can then use this result to subset another list, as you will do in this exercise.

Q&A:
1. Identify the index of max_price in the list prices.
2. Use this index on the names list to identify the company with maximum stock price.

```python 
# Do not modify this
max_price = max(prices)

# Identify index of max price
max_index = prices.index(max_price)

# Identify the name of the company with max price
max_stock_name = names[max_index]

# Fill in the blanks 
print('The largest stock price is associated with ' + max_stock_name + ' and is $' + str(max_price) + '.')
```
### Arrays
#### Installing packages
```python 
pip3 install package_name_herepip3 install numpy
```
```python 
pip3 install numpy
```
#### Numpy arrays
##### NumPy and Arrays
```python 
import numpy
my_array = numpy.array([0, 1, 2, 3, 4])
print(my_array)
[0, 1, 2, 3, 4]
print(type(my_array))
<class 'numpy.ndarray'>

```
##### Using an alias
```python 
import numpy as np
my_array = np.array([0, 1, 2, 3, 4])
print(my_array)

[0, 1, 2, 3, 4]

```
##### Why use an array for financial analysis?
Arrays can handle very large datasets;
- Computationally-memory efficient
- Faster calculations and analysis than lists
- Diverse functionality (many functions in Python packages)

#### What's the difference?
##### NUMPY ARRAYS


##### Create an array
You can use the NumPy package to create arrays. NumPy arrays are optimized for numerical analyses and contain only a single data type. To convert a list to an array, you can use the array() function from NumPy.
```python 
mport numpy as np

a_list = [1, 2, 3, 4]
a_list

[1, 2, 3, 4]

an_array = np.array(a_list)
an_array

array([1, 2, 3, 4])
```
Q&A:
1. Import numpy using the alias np.
2. Create prices_array and earnings_array arrays from the lists prices and earnings, respectively.
```python 
# Import numpy as np
import numpy as np

# Lists
prices = [170.12, 93.29, 55.28, 145.30, 171.81, 59.50, 100.50]
earnings = [9.2, 5.31, 2.41, 5.91, 15.42, 2.51, 6.79]

# NumPy arrays
prices_array = np.array(prices)
earnings_array = np.array(earnings)
```
```
[170.12  93.29  55.28 145.3  171.81  59.5  100.5 ]
[ 9.2   5.31  2.41  5.91 15.42  2.51  6.79]
```
##### Elementwise operations on arrays
Arrays allow for efficient numerical manipulation of its elements. Let's explore element-wise mathematical operations by calculating price to earnings ratio using two arrays, prices_array and earnings_array from the previous exercise.

This price to earnings ratio, or PE ratio, is a financial indicator of the dollar amount an investor can expect to invest in a company in order to receive one dollar of that company’s earnings.

Q&A:
1. import numpy as np.
2. Create pe_array by dividing prices_array by earnings_array.

```python 
# Import numpy as np
import numpy as np

# Create PE ratio array
pe_array = prices_array/ earnings_array

# Print pe_array
print(pe_array)

```

##### Subsetting elements from an array

Subsetting arrays is similar to subsetting lists.

Q&A:
1. Subset the first three elements from prices_array.

```python 
# Subset the first three elements
prices_subset_1 = prices_array[0:3]
print(prices_subset_1)
```

2. Subset the last three elements from the prices_array using negative index slicing.

```python 
# Subset last three elements 
prices_subset_2 = prices_array[-3:]
print(prices_subset_2)
```
3. Subset every third element from the prices_array using step slicing.

```python 
# Subset every third element
prices_subset_3 = prices_array[0:7:3]
print(prices_subset_3)
```
#### Two dimensional arrays

##### Creating a 2D array
Multi-dimensional arrays can be useful for several tasks. In finance, for example, a 2D array may be used to store the prices and earnings for various companies. 

Q&A:
1. Create a two dimensional array of prices and earnings (in that order) and assign it to stock_array.
