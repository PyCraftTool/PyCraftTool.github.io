---
layout: default
---


# Table of Contents

Below, we present four supplementary materials:

1. [Tool](/#1-tool)
2. [Dataset](/#2-dataset)
3. [Patch Submission](/#3-patch-submission)
4. [Supplemental Plots](/#4-supplemental-plots)

# 1. Tool
The tool, along with installation and usage instructions can be found [here](https://github.com/PyCraftTool/PyCraft).

# 2. Dataset

## Table 1
The table below adds details to the table-1 described in the paper. 

Please **scroll** right to view the entire table.

Each number inside the table links to a JSON list 
containing the corresponding data. Each element in the JSON
list is a piece of code, in the form of a string.

Here is a sample JSON list:
```
[
 "count = 0\nfor i in int_list:\n    count += i",
 "import numpy as np\ncount = np.sum(int_list)",
 "count = sum(int_list)",
 .
 .
 .
]
```


<div style="overflow-x:scroll">
<table>
    <tr>
        <th rowspan="2">CPAT Number</th>
        <th rowspan="2">CPAT Name</th>
        <th rowspan="2">LHS</th>
        <th rowspan="2">RHS</th>
        <th colspan="4" style="text-align:center">Variants</th>
    </tr>
    <tr>
        <th style="font-size:13px">Total</th>
        <th style="font-size:13px">Correct</th>
        <th style="font-size:13px">Useful </th>
        <th style="font-size:13px"> Applicable</th>
    </tr>
    <tr>
<td>1</td><td>numpy-sum</td>
<td>

<pre style="width:200px; overflow:auto">
count = 0
for i in int_list:
   count = count + i
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
<td>2</td><td>dict-update</td>
<td>

<pre style="width:200px; overflow:auto">
for k, v in add_dict.items():
    d[k] = v 
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
<td>3</td><td>set-intersection</td>
<td>

<pre style="width:200px; overflow:auto">
common = []
for i in l1:
    if i in l2 and i not in common:
        common.append(i)
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
<td>4</td><td>string-join</td>
<td>

<pre style="width:200px; overflow:auto">
string = "["
for idx, item in enumerate(values):
    if idx != 0:
        string += ", "
    string += item
string += "]"
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
<td>5</td><td>dict-setdefault</td>
<td>

<pre style="width:200px; overflow:auto">
d = {}
for i in array:
  if i in d:
    d[i].append(f(i))
  else:
    d[i] = [f(i)]
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
<td>6</td><td>collections-counter</td>
<td>

<pre style="width:200px; overflow:auto">
counts = {}
for i in iterable:
    if i not in counts:
        counts[i] = 0
    counts[i] += 1
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
<td>7</td><td>numpy-cumsum</td>
<td>

<pre style="width:200px; overflow:auto">
cum_arr = []
for i in range(len(array)):
    cum_arr.append(sum(array[:i+1]))
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
<td>8</td><td>numpy-dot</td>
<td>

<pre style="width:200px; overflow:auto">
dot_prod = 0
for i in range(len(arr1)):
    dot_prod += arr1[i] * arr2[i]
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
<td>9</td><td>numpy-add</td>
<td>

<pre style="width:200px; overflow:auto">
result = []
for i in range(len(array1)):
    result.append(array1[i] + array2[i])
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
<td>10</td><td>list-comprehension</td>
<td>

<pre style="width:200px; overflow:auto">
t = []
for i in range(len(elem)):
    if cond(elem[i]):
         t.append(elem[i])  
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
<td>11</td><td>context-manager-tempfile</td>
<td>

<pre style="width:200px; overflow:auto">
import tempfile
temp_dir = tempfile.TemporaryDirectory()
file=temp_dir.name+"/features.json"
f=open(file, 'w')
f.write(content)
temp_dir.cleanup()
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
- </td>
<td>
-</td>
    </tr>


<tr>
<td>12</td><td>np-mean</td>
<td>

<pre style="width:200px; overflow:auto">
mean = sum(arr1)/len(arr1)
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
- </td>
<td>
-</td>
    </tr>


<tr>
<td>13</td><td>np-multidot</td>
<td>

<pre style="width:200px; overflow:auto">
import numpy as np
result = np.dot(np.dot(arr1, arr2), arr3)
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
- </td>
<td>
-</td>
    </tr>


<tr>
<td>14</td><td>assign-multiple-targets</td>
<td>

<pre style="width:200px; overflow:auto">
a=x
b=y
c=z
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
- </td>
<td>
-</td>
    </tr>

<tr>
<td>15</td><td>swapping-variables</td>
<td>

<pre style="width:200px; overflow:auto">
temp = a
a = b
b = temp
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
- </td>
<td>
-</td>
    </tr>

<tr>
<td>16</td><td>non-zero-compare</td>
<td>

<pre style="width:200px; overflow:auto">
val=val1
if (number_value!=0):
     val=val2
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
- </td>
<td>
-</td>
    </tr>

<tr>
<td>17</td><td>getattr</td>
<td>

<pre style="width:200px; overflow:auto">
try:
  n = obj.name
except:
  n = "unknown"
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
- </td>
<td>
-</td>
    </tr>

<tr>
<td>18</td><td>is-instance</td>
<td>

<pre style="width:200px; overflow:auto">
val=val1
if type(int_instance) is int:
    val=val2
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
- </td>
<td>
-</td>
    </tr>
<tr>
<td>19</td><td>file-context-manager</td>
<td>

<pre style="width:200px; overflow:auto">
file = open(file_path, 'r')
contents = file.read()
file.close()
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
- </td>
<td>
-</td>
    </tr>
<tr>
<td>20</td><td>any-func</td>
<td>

<pre style="width:200px; overflow:auto">
if(c1 or c2 or c3 or c4):
  value = val1
else:
  value = val2
</pre>

</td>
<td>

<pre style="width:200px; overflow:auto">
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
- </td>
<td>
-</td>
    </tr>
</table>
</div>

## RQ1
In [RQ1](/rq1), we quantitatively
assess the ability of LLMs to generate variants.

## RQ2
In [RQ2](/rq2), we quantitatively
assess the ability of LLMs to generate testcases.


## RQ3
In this research question, we find the best performing parameters
for generating variants (gpt-3.5). Below, we provide the oracle used to make these decisions.

Each csv file linked below contains these 4 columns:
1. 'variant': The variant generated by the LLM
2. 'temperature-iterations': The temperature, iterations settings used to generate the variant
3. 'useful': True/False value indicating whether a real developer would write such a variant.
4. 'applicable': Aligns with the intent of the CPAT and is 'useful'

 
### Data:

* [CPAT-1](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/numpy-sum.csv)
* [CPAT-2](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/dict-update.csv)
* [CPAT-3](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/set-intersection.csv)
* [CPAT-4](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/string-join.csv)
* [CPAT-5](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/dict-setdefault.csv)
* [CPAT-6](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/collections-counter.csv)
* [CPAT-7](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/numpy-cumsum.csv)
* [CPAT-8](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/numpy-dot.csv)
* [CPAT-9](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/numpy-add.csv)
* [CPAT-10](https://github.com/PyCraftTool/PyCraft/blob/main/data/paper/RQ3/list-comprehension.csv)

## RQ4
In this research question, we find the best performing parameters
for generating testcases (gpt-3.5).

The links below contain data in the form of a JSON list. Each element 
of the list contains a JSON object which represents a test case.
Here is an example:

```
[
  {
    "init": "int_list=[]",
    "assertion": "assert count == 0"
  },
  .
  .
  .
]  
```

The key "init" contains a piece of code to initialise the input
variables. The key "assertion" contains assertion statements to 
validate the correctness of the variant.


Handwritten test cases can be found [here](https://github.com/PyCraftTool/PyCraft/tree/main/data/paper/RQ4/manual_tests). 
These tests were used to benchmark the performance of LLMs.

Testcases generated by [GPT-3.5](https://github.com/PyCraftTool/PyCraft/tree/main/data/paper/RQ4/gpt-3.5-turbo)

Testcases generated by [GPT-4](https://github.com/PyCraftTool/PyCraft/tree/main/data/paper/RQ4/gpt-4)

 
# 3. Patch Submission

We submitted refactoring patches to open source. 
Below is the status of the pull requests we submitted.

| Repository                                     | Pull Request Link                                                                    | Status   |
|:-----------------------------------------------|:-------------------------------------------------------------------------------------|:---------|
| tosemml/featuretools                           | [pull/1](https://github.com/tosemml/featuretools/pull/1  )                           | Approved |
| matciotola/Z-PNN                               | [pull/4](https://github.com/matciotola/Z-PNN/pull/4  )                               | Approved |
| alexandra-chron/hierarchical-domain-adaptation | [pull/7](https://github.com/alexandra-chron/hierarchical-domain-adaptation/pull/7  ) | Approved |
| chrhenning/hypnettorch                         | [pull/7](https://github.com/chrhenning/hypnettorch/pull/7  )                         | Approved |
| Beyond-ML-Labs/BeyondML                        | [pull/43](https://github.com/Beyond-ML-Labs/BeyondML/pull/43  )                      | Approved |
| StanleyLsx/entity_extractor_by_pointer         | [pull/8](https://github.com/StanleyLsx/entity_extractor_by_pointer/pull/8  )         | Approved |
| ChrisWu1997/DeepCAD                            | [pull/16](https://github.com/ChrisWu1997/DeepCAD/pull/16  )                          | Approved |
| githubharald/SimpleHTR                         | [pull/164](https://github.com/githubharald/SimpleHTR/pull/164  )                     | Approved |
| mlcommons/GaNDLF                               | [pull/719](https://github.com/mlcommons/GaNDLF/pull/719  )                           | Approved |
| NeuroTorch/NeuroTorch                          | [pull/140](https://github.com/NeuroTorch/NeuroTorch/pull/140  )                      | Approved |
| nod-ai/SHARK                                   | [pull/1817](https://github.com/nod-ai/SHARK/pull/1817  )                             | Approved |
| Spico197/DocEE                                 | [pull/67](https://github.com/Spico197/DocEE/pull/67  )                               | Approved |
| undertheseanlp/underthesea                     | [pull/713](https://github.com/undertheseanlp/underthesea/pull/713  )                 | Approved |
| alteryx/featuretools                           | [pull/2607](https://github.com/alteryx/featuretools/pull/2607  )                     | Approved |
| akkana/scripts                                 | [pull/27](https://github.com/akkana/scripts/pull/27  )                               | Approved |
| IDEA-Research/detrex                           | [pull/305](https://github.com/IDEA-Research/detrex/pull/305  )                       | Approved |
| microsoft/DeepSpeed                            | [pull/4262](https://github.com/microsoft/DeepSpeed/pull/4262  )                      | Approved |
| EdisonLeeeee/GreatX                            | [pull/13](https://github.com/EdisonLeeeee/GreatX/pull/13  )                          | Approved |
| shibing624/similarities                        | [pull/15](https://github.com/shibing624/similarities/pull/15  )                      | Approved |
| lucidrains/audiolm-pytorch                     | [pull/228](https://github.com/lucidrains/audiolm-pytorch/pull/228  )                 | Approved |
| artitw/text2text                               | [pull/42](https://github.com/artitw/text2text/pull/42  )                             | Approved |
| microsoft/archai                               | [pull/245](https://github.com/microsoft/archai/pull/245  )                           | Approved |
| autonomousvision/unimatch                      | [pull/33](https://github.com/autonomousvision/unimatch/pull/33  )                    | Approved |
| AlexsLemonade/refinebio                        | [pull/3369](https://github.com/AlexsLemonade/refinebio/pull/3369  )                  | Approved |
| airaria/TextPruner                             | [pull/18](https://github.com/airaria/TextPruner/pull/18  )                           | Approved |
| IBM/inFairness                                 | [pull/68](https://github.com/IBM/inFairness/pull/68  )                               | Approved |
| opendr-eu/opendr                               | [pull/455](https://github.com/opendr-eu/opendr/pull/455  )                           | Approved |
| mit-han-lab/proxylessnas                       | [pull/10](https://github.com/mit-han-lab/proxylessnas/pull/10  )                     | Approved |
| BYU-PRISM/GEKKO                                | [pull/168](https://github.com/BYU-PRISM/GEKKO/pull/168  )                            | Approved |
| TheAlgorithms/Python                           | [pull/8987](https://github.com/TheAlgorithms/Python/pull/8987  )                     | Approved |
| SPFlow/SPFlow                                  | [pull/133](https://github.com/SPFlow/SPFlow/pull/133  )                              | Approved |
| nltk/nltk                                      | [pull/3183](https://github.com/nltk/nltk/pull/3183)                                  | OPEN     |
| pytorch/audio                                  | [pull/3576](https://github.com/pytorch/audio/pull/3576)                              | OPEN     |
| pytorch/tutorials                              | [pull/2547](https://github.com/pytorch/tutorials/pull/2547)                          | OPEN     |
| pytorch/torchrec                               | [pull/1373](https://github.com/pytorch/torchrec/pull/1373)                           | OPEN     |
| microsoft/MMdnn                                | [pull/945](https://github.com/microsoft/MMdnn/pull/945)                              | OPEN     |
| NVIDIA-Merlin/NVTabular                        | [pull/1861](https://github.com/NVIDIA-Merlin/NVTabular/pull/1861)                    | OPEN     |
| dmlc/dgl                                       | [pull/6285](https://github.com/dmlc/dgl/pull/6285)                                   | OPEN     |
| xlang-ai/UnifiedSKG                            | [pull/40](https://github.com/xlang-ai/UnifiedSKG/pull/40 )                           | CLOSED   |
| netsharecmu/NetShare                           | [pull/32](https://github.com/netsharecmu/NetShare/pull/32)                           | CLOSED   |
| keras-team/keras                               | [pull/18360](https://github.com/keras-team/keras/pull/18360)                         | CLOSED   |





# 4. Supplemental Plots
Supplemental plots can be found [here](/plots).

We provide additional plots for [Figure 5](/plots#figure-5) and [Figure 7](/plots#figure-7) in the paper.
