## Python newbie

* What data type supported in Python and which of them are mutable?
  What function can you use to check that a certain data type is mutable?

```
The mutable data types are:

    List
    Dictionary
    Set
    
The immutable data types are:

    Numbers (int, float, ...)
    String
    Bool
    Tuple

The id function can be used to check if a given variable is mutable or not.
```

* What is PEP8? Give an example of 5 style guidelines

```
PEP8 is a list of coding conventions and style guidelines for Python

5 style guidelines:

    1. Limit all lines to a maximum of 79 characters.
    2. Surround top-level function and class definitions with two blank lines.
    3. Use commas when making a tuple of one element
    4. Use spaces (and not tabs) for indentation
    5. Use 4 spaces per indentation level
```

* What is the difference between lists and tuples?

```
* Lists are mutable while tuples are immutable
* Lists are slower compared to tuples (you can use timeit to verify)
```

* What is a list comprehension?
  When would you NOT use list comprehension?

```
A concise way for creating lists. Usually faster than the common way
for creating lists since it's not loading the append attribute every iteration.

We would probably not use it of the logic is too long in a way it becomes unreadable
to read the list comprehension implementation.
```

* What _ is used for in Python?

```
1. Translation lookup in i18n
2. Hold the result of the last executed expression or statement
3. As a general purpose "throwaway" variable name. For example: x, y, _ = get_data() (x and y are used but since we don't care about third variable, we "threw it away").
```

* Sort a list of lists by the second item of each nested list

```
li = [[1, 4], [2, 1], [3, 9], [4, 2], [4, 5]]

sorted(x, key=lambda l: l[1])
```

* You have the following lists: [{'name': 'Mario', 'food': ['mushrooms', 'goombas']}, {'name': 'Luigi', 'food': ['mushrooms', 'turtles']}]
  Extract all type of foods. Final output should be: {'mushrooms', 'goombas', 'turtles'}

```
set([food for bro in x for food in bro['food']])
```
