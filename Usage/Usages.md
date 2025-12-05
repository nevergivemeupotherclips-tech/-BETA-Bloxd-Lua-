## functions
### print
```js
/**
 * @param {string} message - The message It calls
 * @param {color} color - It calls the Message with a color
 * @return {void}
*/
print(string,color)

// example:
print("Hello!", { color: "#00FF00" })
```
### warn
```js
/**
 * @param {string} warn - The warn It calls
 * @param {color} color - It calls the Warn with a color
 * @return {void}
*/
warn(string,color)

// example:
warn("Aw!", { color: "#FFA500" })
```
### error
```js
/**
 * @param {string} error - Throws the error at the player!
 * @return {void}
*/
error(error)

// example:
error("Something broke!")
```
## More
### wait
```js
wait(1, function() {
    print("1 second passed!")
})
```
### localTable,and
```js
var t = localTable()
t.name = "stealprooo_"
t.score = 100
if (and(t.score >= 100, t.name)) {
    print("good")
}
```
###  math.random,forNumber
```js
var r = math.random(1, 10)
print(r)
forNumber(1, 5, 1, function(i) {
    print("Index: " + i)
})
```
### whileLoop
```js
var x = 0

whileLoop(
    function() { return x < 3 },
    function() { print(x); x = x + 1 }
)
```
### repeatUntil
```js
var c = 0

repeatUntil(
    function() { print(c); c = c + 1 },
    function() { return c >= 3 }
)
```
### localTable,pairs
```js
var t = localTable()
t.a = 10
t.b = 20

pairs(t, function(key, value) {
    print(key + ": " + value)
})
```
### ipairs
```js
var arr = [10, 20, 30]

ipairs(arr, function(i, v) {
    print(i + " = " + v)
})
```
