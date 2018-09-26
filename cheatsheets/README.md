# Cheat Sheets


* Sort nested lists or tuples by second item

```
li = [[1, 4], [2, 1], [3, 9], [4, 2], [4, 5]]

sorted(x, key=lambda l: l[1])
```

* Iterate over a dictionary

```
Python 3:
for key, value in d.items():

Python 2:
for key, value in d.iteritems():
```

* Iterate with a counter

```
for count, item in enumerate(some_list):
```
