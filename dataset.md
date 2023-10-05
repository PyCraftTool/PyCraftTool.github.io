---
layout: default
---

# Dataset
Here, we describe and detail the data used to 
back our findings in various research questions.

## RQ1
In this research question, we quantitatively
assess the ability of LLMs to generate variants.

## RQ2
In this research question, we quantitatively
assess the ability of LLMs to generate testcases.

## RQ3
In this research question, we find the best performing parameters
for generating variants (gpt-3.5)
<table>
    <tr>
        <td>CPAT Number</td>
        <td>LHS</td>
        <td>RHS</td>
        <td>Total Variants</td>
        <td>Correct Variants</td>
        <td>Useful Variants</td>
        <td>Applicable Variants</td>
    </tr>
    <tr>
<td>1</td>
<td>

```python
count = 0
for i in int_list:
   count = count + i
```

</td>
<td>

```python
import numpy as np
count = np.sum(int_list)
```

</td>
<td>1185</td>
<td>291</td>
<td>83</td>
<td>50</td>
    </tr>
    <tr>
<td>2</td>
<td>

```python
for k, v in add_dict.items():
    d[k] = v 
```

</td>
<td>

```python
d.update(add_dict)
```

</td>
<td>1201</td>
<td>478</td>
<td>119</td>
<td>110</td>
    </tr>
    <tr>
<td>3</td>
<td>

```python
common = []
for i in l1:
    if i in l2 and i not in common:
        common.append(i)
```

</td>
<td>

```python
common = list(set(l1).
            intersection(l2))
```

</td>
<td>782 </td>
<td>287 </td>
<td>107 </td>
<td>66</td>
    </tr>
    <tr>
<td>4</td>
<td>

```python
string = "["
for idx, item in enumerate(values):
    if idx != 0:
        string += ", "
    string += item
string += "]"
```

</td>
<td>

```python
string = "[" + ", ".join(values)+ "]"
```

</td>
<td>285 </td>
<td>101 </td>
<td>20</td>
<td>10</td>
    </tr>
    <tr>
<td>5</td>
<td>

```python
d = {}
for i in array:
  if i in d:
    d[i].append(f(i))
  else:
    d[i] = [f(i)]
```

</td>
<td>

```python
d = {}
for i in array:
    d.setdefault(i, []).append(f(i))
```

</td>
<td>1265 </td>
<td>416 </td>
<td>150</td>
<td>75</td>
    </tr>
    <tr>
<td>6</td>
<td>

```python
counts = {}
for i in iterable:
    if i not in counts:
        counts[i] = 0
    counts[i] += 1
```

</td>
<td>

```python
from collections import Counter
counts = Counter(iterable)
```

</td>
<td>927 </td>
<td>425</td>
<td>202 </td>
<td>85</td>
    </tr>
    <tr>
<td>7</td>
<td>

```python
cum_arr = []
for i in range(len(array)):
    cum_arr.append(sum(array[:i+1]))
```

</td>
<td>

```python
import numpy as np
cum_arr = np.cumsum(array)
```

</td>
<td>1223</td>
<td>290 </td>
<td>95 </td>
<td>80</td>
    </tr>
    <tr>
<td>8</td>
<td>

```python
dot_prod = 0
for i in range(len(arr1)):
    dot_prod += arr1[i] * arr2[i]
```

</td>
<td>

```python
import numpy as np
dot_prod = np.dot(arr1, arr2)
```

</td>
<td>177 </td>
<td>28 </td>
<td>26 </td>
<td>24</td>
    </tr>
    <tr>
<td>9</td>
<td>

```python
result = []
for i in range(len(array1)):
    result.append(array1[i] + array2[i])
```

</td>
<td>

```python
import numpy as np
result = np.add(array1, array2)
```

</td>
<td>64 </td>
<td>11</td>
<td>11 </td>
<td>9</td>
    </tr>
    <tr>
<td>10</td>
<td>

```python
t = []
for i in range(len(elem)):
    if cond(elem[i]):
         t.append(elem[i])  
```

</td>
<td>

```python
t = [elem[i] for i in range(len(elem)) 
        if cond(elem[i])]
```

</td>
<td>955 </td>
<td>453 </td>
<td>226  </td>
<td>71 </td>
    </tr>
</table>