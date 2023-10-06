# RQ1

## GPT-3.5

| CPAT                     | #correct | invalid_format | #type-err | #syntax-err | #import-err | #incorrect |
|--------------------------|----------|----------------|-----------|-------------|-------------|------------|
| context-manager-tempfile | 150      | 0              | 63        | 0           | 81          | 230        |
| assign-multiple-targets  | 11       | 0              | 0         | 0           | 83          | 343        |
| numpy-cumsum             | 61       | 0              | 204       | 0           | 78          | 193        |
| is-instance              | 39       | 0              | 0         | 0           | 57          | 369        |
| swapping-variables       | 77       | 1              | 0         | 0           | 32          | 276        |
| any-func                 | 136      | 2              | 0         | 0           | 2           | 296        |
| numpy-dot                | 18       | 0              | 203       | 0           | 62          | 96         |
| np-mean                  | 97       | 0              | 254       | 0           | 67          | 64         |
| string-join              | 11       | 1              | 279       | 0           | 20          | 145        |
| list-comprehension       | 100      | 0              | 45        | 0           | 43          | 295        |
| collections-counter      | 71       | 0              | 242       | 0           | 12          | 169        |
| set-intersection         | 39       | 0              | 0         | 0           | 34          | 327        |
| dict-setdefault          | 100      | 2              | 161       | 0           | 32          | 215        |
| non-zero-compare         | 69       | 1              | 0         | 0           | 10          | 327        |
| numpy-sum                | 40       | 0              | 286       | 0           | 47          | 100        |
| np-multidot              | 0        | 2              | 0         | 0           | 316         | 123        |
| numpy-add                | 9        | 2              | 158       | 0           | 27          | 281        |
| dict-update              | 102      | 1              | 147       | 0           | 14          | 168        |
| file-context-manager     | 20       | 0              | 127       | 0           | 11          | 407        |
| getattr                  | 109      | 0              | 0         | 0           | 9           | 333        |


## GPT-4

| CPAT                     | #correct | invalid_format | #type-err | #syntax-err | #import-err | #incorrect |
|--------------------------|----------|----------------|-----------|-------------|-------------|------------|
| context-manager-tempfile | 115      | 0              | 37        | 0           | 31          | 252        |
| assign-multiple-targets  | 272      | 0              | 0         | 0           | 16          | 152        |
| numpy-cumsum             | 53       | 3              | 229       | 0           | 10          | 103        |
| is-instance              | 166      | 3              | 0         | 0           | 9           | 219        |
| swapping-variables       | 132      | 3              | 0         | 0           | 20          | 293        |
| any-func                 | 153      | 0              | 0         | 0           | 23          | 247        |
| numpy-dot                | 21       | 0              | 210       | 0           | 27          | 89         |
| np-mean                  | 98       | 0              | 274       | 0           | 20          | 11         |
| string-join              | 101      | 0              | 150       | 0           | 18          | 114        |
| list-comprehension       | 184      | 0              | 30        | 0           | 23          | 196        |
| collections-counter      | 161      | 0              | 113       | 0           | 27          | 136        |
| set-intersection         | 58       | 1              | 0         | 0           | 18          | 268        |
| dict-setdefault          | 132      | 2              | 107       | 0           | 26          | 192        |
| non-zero-compare         | 224      | 20             | 0         | 0           | 7           | 119        |
| numpy-sum                | 67       | 0              | 159       | 0           | 27          | 116        |
| np-multidot              | 0        | 0              | 0         | 0           | 312         | 106        |
| numpy-add                | 15       | 1              | 165       | 0           | 31          | 135        |
| dict-update              | 187      | 0              | 45        | 0           | 15          | 162        |
| file-context-manager     | 144      | 0              | 52        | 0           | 16          | 153        |
| getattr                  | 101      | 0              | 0         | 0           | 6           | 271        |


## PALM

| CPAT                     | #correct | invalid_format | #type-err | #syntax-err | #import-err | #incorrect |
|--------------------------|----------|----------------|-----------|-------------|-------------|------------|
| context-manager-tempfile | 7        | 0              | 36        | 66          | 254         | 164        |
| assign-multiple-targets  | 18       | 0              | 0         | 42          | 104         | 329        |
| numpy-cumsum             | 21       | 0              | 94        | 36          | 121         | 135        |
| is-instance              | 71       | 0              | 0         | 49          | 26          | 341        |
| swapping-variables       | 10       | 0              | 0         | 86          | 36          | 253        |
| any-func                 | 25       | 0              | 0         | 39          | 4           | 422        |
| numpy-dot                | 12       | 0              | 130       | 114         | 111         | 128        |
| np-mean                  | 29       | 0              | 132       | 92          | 184         | 96         |
| string-join              | 3        | 0              | 172       | 26          | 10          | 233        |
| list-comprehension       | 32       | 0              | 82        | 3           | 81          | 332        |
| collections-counter      | 40       | 0              | 41        | 35          | 141         | 256        |
| set-intersection         | 18       | 0              | 0         | 11          | 116         | 370        |
| dict-setdefault          | 34       | 0              | 166       | 38          | 115         | 159        |
| non-zero-compare         | 34       | 0              | 0         | 53          | 56          | 324        |
| numpy-sum                | 27       | 0              | 154       | 123         | 61          | 133        |
| np-multidot              | 0        | 0              | 0         | 27          | 357         | 91         |
| numpy-add                | 13       | 0              | 137       | 43          | 65          | 139        |
| dict-update              | 36       | 0              | 177       | 68          | 29          | 195        |
| file-context-manager     | 0        | 0              | 225       | 107         | 169         | 70         |
| getattr                  | 31       | 0              | 0         | 31          | 38          | 439        |
