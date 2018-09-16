# Python Code Snippets

Useful Python Code Snippets, mainly for Machine Learning algorithms.

### Download file
```python
try:
    from urllib.request import urlretrieve
except ImportError:
    from urllib import urlretrieve
urlretrieve('http://files.grouplens.org/datasets/movielens/ml-1m.zip', 'ml-1m.zip')
assert os.system('unzip -o ml-1m.zip') == 0, 'MovieLens dataset should be downloaded and unziped correctly'
```
### Execute system command
```python
os.system('[command]')
# Executing and checking the result
assert os.system('unzip -o ml-1m.zip') == 0, 'MovieLens dataset should be downloaded and unziped correctly'
```
