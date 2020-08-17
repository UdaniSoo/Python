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

