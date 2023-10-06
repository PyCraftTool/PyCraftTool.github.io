---
layout: default
---

# Dataset
Here, we describe and detail the data used to 
back our findings in various research questions.

## Table 1
The table below adds details to the _table 1_ 
described in the paper.
<div style="overflow-x:scroll">
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

<pre>
count = 0
for i in int_list:
   count = count + i
</pre>

</td>
<td>

<pre>
import numpy as np
count = np.sum(int_list)
</pre>

</td>
<td> <a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/numpy-sum/all_variants.json">1185</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/numpy-sum/correct_variants.json">
291
</a>
</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/numpy-sum/useful_variants.json">
83</a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/numpy-sum/applicable_variants.json">
50</a></td>
    </tr>
    <tr>
<td>2</td>
<td>

<pre>
for k, v in add_dict.items():
    d[k] = v 
</pre>

</td>
<td>

<pre>
d.update(add_dict)
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/dict-update/all_variants.json">
1201</a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/dict-update/correct_variants.json">
478</a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/dict-update/useful_variants.json">
119</a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/dict-update/applicable_variants.json">
110</a></td>
    </tr>
    <tr>
<td>3</td>
<td>

<pre>
common = []
for i in l1:
    if i in l2 and i not in common:
        common.append(i)
</pre>

</td>
<td>

<pre>
common = list(set(l1).
            intersection(l2))
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/set-intersection/all_variants.json">
782 </a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/set-intersection/correct_variants.json">
287</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/set-intersection/useful_variants.json">
107 </a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/set-intersection/applicable_variants.json">
66</a></td>
    </tr>
    <tr>
<td>4</td>
<td>

<pre>
string = "["
for idx, item in enumerate(values):
    if idx != 0:
        string += ", "
    string += item
string += "]"
</pre>

</td>
<td>

<pre>
string = "[" + ", ".join(values)+ "]"
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/string-join/all_variants.json">
285 </a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/string-join/correct_variants.json">
101</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/string-join/useful_variants.json">
20</a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/string-join/applicable_variants.json">
10</a></td>
    </tr>
    <tr>
<td>5</td>
<td>

<pre>
d = {}
for i in array:
  if i in d:
    d[i].append(f(i))
  else:
    d[i] = [f(i)]
</pre>

</td>
<td>

<pre>
d = {}
for i in array:
    d.setdefault(i, []).append(f(i))
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/dict-setdefault/all_variants.json">
1265 </a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/dict-setdefault/correct_variants.json">
416</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/dict-setdefault/useful_variants.json">
150</a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/dict-setdefault/applicable_variants.json">
75</a></td>
    </tr>
    <tr>
<td>6</td>
<td>

<pre>
counts = {}
for i in iterable:
    if i not in counts:
        counts[i] = 0
    counts[i] += 1
</pre>

</td>
<td>

<pre>
from collections import Counter
counts = Counter(iterable)
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/collections-counter/all_variants.json">
927 </a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/collections-counter/correct_variants.json">
425</a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/collections-counter/useful_variants.json">
202</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/collections-counter/applicable_variants.json">
85</a></td>
    </tr>
    <tr>
<td>7</td>
<td>

<pre>
cum_arr = []
for i in range(len(array)):
    cum_arr.append(sum(array[:i+1]))
</pre>

</td>
<td>

<pre>
import numpy as np
cum_arr = np.cumsum(array)
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/numpy-cumsum/all_variants.json">
1223</a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/numpy-cumsum/correct_variants.json">
290 </a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/numpy-cumsum/useful_variants.json">
95 </a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/numpy-cumsum/applicable_variants.json">
80</a></td>
    </tr>
    <tr>
<td>8</td>
<td>

<pre>
dot_prod = 0
for i in range(len(arr1)):
    dot_prod += arr1[i] * arr2[i]
</pre>

</td>
<td>

<pre>
import numpy as np
dot_prod = np.dot(arr1, arr2)
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/numpy-dot/all_variants.json">
177 </a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/numpy-dot/correct_variants.json">
28 </a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/numpy-dot/useful_variants.json">
26</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/numpy-dot/applicable_variants.json">
24</a></td>
    </tr>
    <tr>
<td>9</td>
<td>

<pre>
result = []
for i in range(len(array1)):
    result.append(array1[i] + array2[i])
</pre>

</td>
<td>

<pre>
import numpy as np
result = np.add(array1, array2)
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/numpy-add/all_variants.json">
64 </a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/numpy-dot/correct_variants.json">
11</a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/numpy-dot/useful_variants.json">
11</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/numpy-dot/applicable_variants.json">
9</a></td>
    </tr>
    <tr>
<td>10</td>
<td>

<pre>
t = []
for i in range(len(elem)):
    if cond(elem[i]):
         t.append(elem[i])  
</pre>

</td>
<td>

<pre>
t = [elem[i] for i in range(len(elem)) 
        if cond(elem[i])]
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/list-comprehension/all_variants.json">
955</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/list-comprehension/correct_variants.json">
453 </a></td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/list-comprehension/useful_variants.json">
226 </a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/list-comprehension/aplicable_variants.json">
71 </a></td>
    </tr>
</table>
</div>
## RQ1
In this research question, we quantitatively
assess the ability of LLMs to generate variants.

## RQ2
In this research question, we quantitatively
assess the ability of LLMs to generate testcases.
[Link](/rq1)

## RQ3
In this research question, we find the best performing parameters
for generating variants (gpt-3.5)

## RQ4
In this research question, we find the best performing parameters
for generating testcases (gpt-3.5)
