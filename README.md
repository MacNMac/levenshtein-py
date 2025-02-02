# levenshtein-python
Compare between two words, and see if it's similar to each other. Using math and logic only, you can adjust the threeshold which is inside the 'compare' function.

### How to modify:
Change the threeshold to your likings, threeshold means the distance between the two words we put. If a distance between two words is 3, and the threeshold is 2; it will return false.
```python
def compare(sub, target, threshold=2): # Adjust the threeshold to any number you want
    distance = levenshtein_distance(sub, target)
    return distance <= threshold
```
