# Verkefni 1
1. null er ekkert og undefined er eitthvað sem hefur ekki verið skilgreint
2. neyðir mann til að muna að nota ; 
3. let virkar bara inní block-inni sem þú gerðir hann í og var virkar allstaðar
4. 
```javascript
function add(a, b) {
    return a + b;
}
var add = function(a, b) {
    return a + b;
};
var add = (a, b) => a + b;
```
5. runnar function sem birtir alert með textanum 'Hello World'
6. útkomur bar function-ina eru vistuð áður en það er kallað í þau svo 3 overwrite-ast sem 8 áður en það er kallað í það
7. 
        for er start; stop; step.
        The for...in statement iterates a specified variable over all the enumerable properties of an object. For each distinct property, JavaScript executes the specified statements.
        The for...of statement creates a loop Iterating over iterable objects (including Array, Map, Set, arguments object and so on), invoking a custom iteration hook with statements to be executed for the value of each distinct property.
8. 
```javascript
var test = [12, 929, 11, 3, 199, 1000, 7, 1, 24, 37, 4,
    19, 300, 3775, 299, 36, 209, 148, 169, 299,
    6, 109, 20, 58, 139, 59, 3, 1, 139
];

// Write your code here
test.forEach(function(element, index) {
  if (element % 3 === 0) {
      test[index] += 100;
  }
});
```
9. 
```javascript
var bills = [50.23, 19.12, 34.01,
    100.11, 12.15, 9.90, 29.11, 12.99,
    10.00, 99.22, 102.20, 100.10, 6.77, 2.22
];

const totals = bills.map(x => Number((x + (x * .15)).toFixed(2)));

console.log(totals)
```
10.
```javascript
var numbers = [
    [243, 12, 23, 12, 45, 45, 78, 66, 223, 3],
    [34, 2, 1, 553, 23, 4, 66, 23, 4, 55],
    [67, 56, 45, 553, 44, 55, 5, 428, 452, 3],
    [12, 31, 55, 445, 79, 44, 674, 224, 4, 21],
    [4, 2, 3, 52, 13, 51, 44, 1, 67, 5],
    [5, 65, 4, 5, 5, 6, 5, 43, 23, 4424],
    [74, 532, 6, 7, 35, 17, 89, 43, 43, 66],
    [53, 6, 89, 10, 23, 52, 111, 44, 109, 80],
    [67, 6, 53, 537, 2, 168, 16, 2, 1, 8],
    [76, 7, 9, 6, 3, 73, 77, 100, 56, 100]
];

// your code goes here
for(let i of numbers) {
    for (let numberIndex in i) {
        if(i[numberIndex] % 2 === 0) {
            i[numberIndex] = "even";
        } else {
          i[numberIndex] = "odd";  
        };
    }
}
```
