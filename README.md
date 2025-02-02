# levenshtein-python
The Levenshtein distance is a string metric for measuring the difference between two sequences. Informally, the Levenshtein distance between two words is the minimum number of single-character edits (i.e. insertions, deletions or substitutions) required to change one word into the other.

### How to modify:
Change the threeshold to your likings, threeshold means the distance between the two words we put. If a distance between two words is 3, and the threeshold is 2; it will return false.
```python
def compare(sub, target, threshold=2): # Adjust the threeshold to any number you want
    distance = levenshtein_distance(sub, target)
    return distance <= threshold
```
Or, you can add some additions to 'compare' function:
```python
    return (distance <= threshold, distance) # So, this lets you know the distance.
```
### Example:
```python
if __name__ == "__main__":
    result = compare("Hello", "help")
    print(result) # False
```
