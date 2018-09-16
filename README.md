# Python Code Snippets

Useful code snippets, mainly for Machine Learning algorithms.

## General

* Download file
```python
try:
    from urllib.request import urlretrieve
except ImportError:
    from urllib import urlretrieve
urlretrieve('http://files.grouplens.org/datasets/movielens/ml-1m.zip', 'ml-1m.zip')
```
* Execute system command
```python
import os
os.system('[command]')
# Executing and checking the result
assert os.system('unzip -o ml-1m.zip') == 0, 'MovieLens dataset should be downloaded and unziped correctly'
```
## Panda
```python
import pandas as pd
```

* Check for null fields
```python
myPandaDs.isnull().sum()
```
* Drop empty rows
```python
myPandaDs = myPandaDs.dropna(axis=0) # axis = 0 means we drop lines
```
* Check if dataset has null fields
```python
movielens1M.isnull().sum()
```
