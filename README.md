# Example Doc Lookup Issue

## Steps to reproduce:

Try documentation lookup on the `Right` on line 5 of _example.scala_

## Expected

The documentation to be found, namely:

```
http://127.0.0.1:57291/docs/cats-core_2.11-0.4.1-javadoc.jar/index.html#cats.data.Xor$$Right
```

## Actual

No documentation found (FalseResponse returned).

# Notes

Exchange logged in Atom ENSIME:

```
outgoing: 0000a8{
  "req": {
    "typehint":"DocUriAtPointReq",
    "file":"/Users/richard/Developer/tmp/xor-scaldoc-lookup/src/main/scala/example.scala",
    "point":{"from":61,"to":61}},
    "callId": 28
  }

incoming: {"callId":28,"payload":{"typehint":"FalseResponse"}}
```
