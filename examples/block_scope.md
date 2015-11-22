```js
function x(a) {
  {
    let a = 4
    let b = 10
    var c = true
    a; //: number
    b; //: number
    c; //: bool
  }
  a; //: string
  b; //: ?
  c; //: bool
}

x("hello")
```
```json
[
  {
    "id": "a4a4f180-90bd-11e5-bbb9-89e85171e4ff",
    "name": "x",
    "addr": "/x/",
    "kind": "f",
    "type": "void function(string)",
    "lineno": 1,
    "origin": {
      "!span": "9[0:9]-10[0:10]",
      "!type": "fn(a: string)",
      "!data": {
        "isConstructor": false,
        "isPlainObject": false
      }
    },
    "tagfile": "__DIR__/block_scope.js"
  },
  {
    "id": "a4a51890-90bd-11e5-bbb9-89e85171e4ff",
    "name": "a",
    "addr": "/a/",
    "kind": "v",
    "type": "string",
    "lineno": 1,
    "namespace": "x",
    "parent": "a4a4f180-90bd-11e5-bbb9-89e85171e4ff",
    "origin": {
      "!span": "11[0:11]-12[0:12]",
      "!type": "string",
      "!data": {
        "isConstructor": false,
        "scoped": true,
        "isArg": true,
        "isPlainObject": false
      }
    },
    "tagfile": "__DIR__/block_scope.js"
  },
  {
    "id": "a4a51891-90bd-11e5-bbb9-89e85171e4ff",
    "name": "c",
    "addr": "/c/",
    "kind": "v",
    "type": "boolean",
    "lineno": 5,
    "namespace": "x",
    "parent": "a4a4f180-90bd-11e5-bbb9-89e85171e4ff",
    "origin": {
      "!span": "57[4:8]-58[4:9]",
      "!type": "bool",
      "!data": {
        "isConstructor": false,
        "scoped": false,
        "isArg": false,
        "isPlainObject": false
      }
    },
    "tagfile": "__DIR__/block_scope.js"
  }
]
```
```ctags
x	__DIR__/block_scope.js	/x/;"	f	lineno:1	type:void function(string)
a	__DIR__/block_scope.js	/a/;"	v	lineno:1	namespace:x	type:string
c	__DIR__/block_scope.js	/c/;"	v	lineno:5	namespace:x	type:boolean
```