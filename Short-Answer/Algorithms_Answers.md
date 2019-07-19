Add your answers to the Algorithms exercises here.

## Exercise 1

---

### a)

```python
a = 0
    while (a < n * n * n):
      a = a + n * n
```

this is a big O algorithm. `O(n)`
First line runs once regaurdless of the `n` value

```
0(1)+ 0(n) \* 0(1) = 0(n)
```

---

### b)

```
sum = 0 # --> O(1)
  for i in range(n): # --> O(n)
  i += 1 # --> O(1)
    for j in range(i + 1, n): # --> O(n)
      j += 1 # --> O(1)
      for k in range(j + 1, n): # --> O(n)
        k += 1 # --> O(1)
        for l in range(k + 1, 10 + k): # --> O(n)
          l += 1 # --> O(1)
          sum += 1 # --> O(1)
```

```
From bottom to the top ---> It is cubic 0(n^3)
```

---

### c)

```
Linear --> 0(n)
```

```
def bunnyEars(bunnies):
if bunnies == 0: # --> O(1)
return 0 # --> O(1)
return 2 + bunnyEars(bunnies-1)O(n)
```

---

## Exercise 2

---

```
n --> n story building (Already ordered)
eggs --> Unlimited
f ---> floor number

# Start at the ground floor i.e., f = 0
f = 0
# Start a loop from f=0 to n(number of stores in the building)
for f in range(0,n):
  # if eggs are broken for a given f then return that "f" value
  if eggs_broken is True:
     return f
  else:
     return None
```
