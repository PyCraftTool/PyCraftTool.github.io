---
layout: default
---

# Table of Contents
1. [Tool](/#1-tool)
2. [Dataset](/#2-dataset)
3. [Supplemental Plots](/#3-supplemental-plots)

# 1. [Tool](https://github.com/PyCraftTool/PyCraft)
The tool, along with installation and usage instructions can be found [here](https://github.com/PyCraftTool/PyCraft).

# 2. Dataset

## Table 1
The table below adds details to the table-1 described in the paper. 

Please **scroll** right to view the entire table.
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


<tr>
<td>11</td>
<td>

<pre>
import tempfile
temp_dir = tempfile.TemporaryDirectory()
file=temp_dir.name+"/features.json"
f=open(file, 'w')
f.write(content)
temp_dir.cleanup()
</pre>

</td>
<td>

<pre>
with tempfile.TemporaryDirectory() as temp_dir:
    file=temp_dir+"/features.json"
    f=open(file, 'w')
    f.write(content)
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/context-manager-tempfile/all_variants.json">
524</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/context-manager-tempfile/correct_variants.json">
150 </a></td>
<td>
<a href="/">
- </a> </td>
<td>
<a href="/">
- </a></td>
    </tr>


<tr>
<td>12</td>
<td>

<pre>
mean = sum(arr1)/len(arr1)
</pre>

</td>
<td>

<pre>
import numpy as np
mean=np.mean(arr1)
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/np-mean/all_variants.json">
482</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/np-mean/correct_variants.json">
97 </a></td>
<td>
<a href="/">
- </a> </td>
<td>
<a href="/">
- </a></td>
    </tr>


<tr>
<td>13</td>
<td>

<pre>
import numpy as np
result = np.dot(np.dot(arr1, arr2), arr3)
</pre>

</td>
<td>

<pre>
import numpy as np
result = np.linalg.multi_dot([arr1, arr2, arr3])
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/np-multidot/all_variants.json">
439</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/np-multidot/correct_variants.json">
0 </a></td>
<td>
<a href="/">
- </a> </td>
<td>
<a href="/">
- </a></td>
    </tr>


<tr>
<td>14</td>
<td>

<pre>
a=x
b=y
c=z
</pre>

</td>
<td>

<pre>
a,b,c = x,y,z
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/assign-multiple-targets/all_variants.json">
437</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/assign-multiple-targets/correct_variants.json">
11 </a></td>
<td>
<a href="/">
- </a> </td>
<td>
<a href="/">
- </a></td>
    </tr>

<tr>
<td>15</td>
<td>

<pre>
temp = a
a = b
b = temp
</pre>

</td>
<td>

<pre>
a,b = b,a
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/swapping-variables/all_variants.json">
385</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/swapping-variables/correct_variants.json">
77 </a></td>
<td>
<a href="/">
- </a> </td>
<td>
<a href="/">
- </a></td>
    </tr>

<tr>
<td>16</td>
<td>

<pre>
val=val1
if (number_value!=0):
     val=val2
</pre>

</td>
<td>

<pre>
val=val1
if (bool(number_value)):
     val=val2
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/non-zero-compare/all_variants.json">
406</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/non-zero-compare/correct_variants.json">
69 </a></td>
<td>
<a href="/">
- </a> </td>
<td>
<a href="/">
- </a></td>
    </tr>

<tr>
<td>17</td>
<td>

<pre>
try:
  n = obj.name
except:
  n = "unknown"
</pre>

</td>
<td>

<pre>
n = getattr(obj, 'name', 'unknown')
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/getattr/all_variants.json">
451</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/getattr/correct_variants.json">
109 </a></td>
<td>
<a href="/">
- </a> </td>
<td>
<a href="/">
- </a></td>
    </tr>

<tr>
<td>18</td>
<td>

<pre>
val=val1
if type(int_instance) is int:
    val=val2
</pre>

</td>
<td>

<pre>
val=val1
if isinstance(int_instance, int):
    val=val2
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/is-instance/all_variants.json">
465</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/is-instance/correct_variants.json">
39 </a></td>
<td>
<a href="/">
- </a> </td>
<td>
<a href="/">
- </a></td>
    </tr>
<tr>
<td>19</td>
<td>

<pre>
file = open(file_path, 'r')
contents = file.read()
file.close()
</pre>

</td>
<td>

<pre>
with open(file_path, 'r') as f:
    contents = f.read()
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/file-context-manager/all_variants.json">
565</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/file-context-manager/correct_variants.json">
20 </a></td>
<td>
<a href="/">
- </a> </td>
<td>
<a href="/">
- </a></td>
    </tr>
<tr>
<td>20</td>
<td>

<pre>
if(c1 or c2 or c3 or c4):
  value = val1
else:
  value = val2
</pre>

</td>
<td>

<pre>
if any((c1,c2,c3,c4)):
  value = val1
else:
  value = val2
</pre>

</td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/any-func/all_variants.json">
434</a> </td>
<td>
<a href="https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/Table1/any-func/correct_variants.json">
136 </a></td>
<td>
<a href="/">
- </a> </td>
<td>
<a href="/">
- </a></td>
    </tr>
</table>
</div>

## [RQ1](/rq1)
In this research question, we quantitatively
assess the ability of LLMs to generate variants.

## [RQ2](/rq2)
In this research question, we quantitatively
assess the ability of LLMs to generate testcases.


## RQ3
In this research question, we find the best performing parameters
for generating variants (gpt-3.5). Below, we provide the oracle used to make these decisions.

Each csv file linked below contains these 4 columns:
1. 'variant': The variant generated by the LLM
2. 'temperature-iterations': The temperature, iterations settings used to generate the variant
3. 'useful': True/False value indicating whether a real developer would write such a variant.
4. 'applicable': Aligns with the intent of the CPAT and is 'useful'

| CPAT                                                                                                           | 
|----------------------------------------------------------------------------------------------------------------|
| [numpy-sum](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/numpy-sum.csv)                     |
| [list-comprehension](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/list-comprehension.csv)   |
| [dict-update](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/dict-update.csv)                 |
| [set-intersection](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/set-intersection.csv)       |
| [string-join](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/string-join.csv)                 |
| [dict-setdefault](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/dict-setdefault.csv)         |
| [collections-counter](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/collections-counter.csv) |
| [numpy-cumsum](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/numpy-cumsum.csv)               |
| [numpy-dot](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/numpy-dot.csv)                     |
| [numpy-add](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/numpy-add.csv)                     |




## RQ4
In this research question, we find the best performing parameters
for generating testcases (gpt-3.5)

Handwritten test cases can be found [here](https://github.com/PyCraftTool/PyCraft/tree/main/data/paper/RQ4/manual_tests). 
These tests were used to benchmark the performance of LLMs.

Testcases generated by [GPT-3.5](https://github.com/PyCraftTool/PyCraft/tree/main/data/paper/RQ4/gpt-3.5-turbo)

Testcases generated by [GPT-4](https://github.com/PyCraftTool/PyCraft/tree/main/data/paper/RQ4/gpt-4)

 




# 3. [Supplemental Plots](/plots)
We provide additional plots for [Figure 5](/plots#figure-5) and [Figure 7](/plots#figure-7) in the paper.
