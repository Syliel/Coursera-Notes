JavaScript Object Notation
* Douglas Crockford "Discovered" JSON 2001
* Object literal notation in JavaScript

```python

import json
data = '''{
"name" : "Chuck",
"phone": {
	"type" : "intl",
	"number" : "+1 734 303 4456"
},
"email" : {
	"hide" : "yes"
}
}'''
info = json.loads(data)
print('Name:', info["name"])
print('Hide:', info["email"]["hide"])

```
* JSON represents data as nested "lists" and "dictionaries"
* Have lists and dictionaries and can be nested anyway you want. 

```python

import json
input = '''[
	{ "id"   : "001", 
	  "x"    : "2",
	  "name" : "Chuck"
	},
	{ "id"   : "009",
	  "x"    : "7",
	  "name" : "Chuck:
	}
	}
]'''

info = json.loads(input)
print('User Count:', len(info))
for item in info:
	print('Name', item['name'])
	print('Id', item['id'])
	print('Attribute', item['x'])
```
