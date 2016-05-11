#Spread Operators
Find max number of values in an array
```javascript
//ES5
const numbers = [2, 4, 8, 64, 128, 256];
const max = Math.max(numbers);
console.log(max); //NaN

//workaround in ES5
const max2 = Math.max.apply(null, numbers);
console.log(max2); //256
```
Using spread operator. The array of the elements are spread out or dispersed.
```javascript
const numbers = [2, 4, 8, 64, 128, 256];
const max = Math.max(...numbers);
console.log(max); //256

```
Spread expands arrays. So, you can expand array in arrays
```javascript
const numbers1 = [1, 2, 3, 4, 5];
const numbers2 = [6, 7, 8, 9, 10];

const allNumbers = [...numbers1, ...numbers2];
console.log(allNumbers);
```
Or concat arrays of strings
```javascript
let europeanCities = ['London', 'Oslo'];
let allCities = ['LA', 'Seatle', ...europeanCities, 'Orlando', 'NYC'];

console.log(allCities);
```