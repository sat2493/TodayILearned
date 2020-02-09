# Assert Equals

TIL that asserts don't exist in JavaScript. However an asserts could be implemented similarly through the following

```
function assert(condition, message) {
    if (!condition) {
        throw message || "Assertion failed";
    }
}
```
