# manually-written-filter-function
 Logic of built-in .filter() function

```javascript
function filterArray(array, callback) {
    const resultingArray = []
    for (let item of array) {
        const shouldBeIncluded = callback(item)
        if (shouldBeIncluded) {
            resultingArray.push(item)
        }
    }
    return resultingArray
}

//This code is about how the .filter() function works in JavaScript.