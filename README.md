runphp
======

Run most of PHP functions from command-line like this:
```bash
$ runphp base64_encode 'mystring'
bXlzdHJpbmc=
```

```bash
# Use json for arrays
$ runphp array_merge [1,2,3] [4,5,6]
Array
(
    [0] => 1
    [1] => 2
    [2] => 3
    [3] => 4
    [4] => 5
    [5] => 6
)
```

```bash
# json output (--output json or -o json)
$ runphp array_merge '{"a": 1, "b": "string"}' '{"c": false, "d": [1,2,3]}' --output json
{"a":1,"b":"string","c":false,"d":[1,2,3]}
```

```bash
$ runphp
"function" required
 runphp function [-o|--output json] [arg1] [arg2] ...
```
