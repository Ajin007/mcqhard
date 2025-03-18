
### Question 1: **What is the output of the following code involving `Date` object manipulation?**
#### Code:
```javascript
const date = new Date('2025-03-15T00:00:00Z');
date.setDate(date.getDate() + 10);
date.setFullYear(date.getFullYear() - 1);
console.log(date.toISOString());
```

#### Options:
A) `2024-03-25T00:00:00.000Z`  
B) `2025-03-25T00:00:00.000Z`  
C) `2025-03-25T10:00:00.000Z`  
D) `2024-03-15T00:00:00.000Z`

#### Answer:
A) `2024-03-25T00:00:00.000Z`

---

### Question 2: **Which of the following methods will generate a random integer between 1 and 100 (inclusive)?**
#### Code:
```javascript
function getRandomInt() {
  return Math.floor(Math.random() * 100) + 1;
}
console.log(getRandomInt());
```

#### Options:
A) It generates a random integer between 1 and 100 (inclusive).  
B) It generates a random float between 1 and 100.  
C) It generates a random integer between 0 and 99.  
D) It generates a random integer between 1 and 99.

#### Answer:
A) It generates a random integer between 1 and 100 (inclusive).

---

### Question 3: **What is the result of this complex async/await operation in the following code?**
#### Code:
```javascript
async function fetchData() {
  let result = 'start';
  try {
    result = await new Promise((resolve, reject) => {
      setTimeout(() => resolve('done'), 2000);
    });
  } catch (error) {
    result = 'error';
  }
  return result;
}

fetchData().then(data => console.log(data));
```

#### Options:
A) `start`  
B) `done`  
C) `error`  
D) `undefined`

#### Answer:
B) `done`

---

### Question 4: **What does the following code with a `setInterval` function do?**
#### Code:
```javascript
let count = 0;
const interval = setInterval(() => {
  count++;
  console.log(count);
  if (count === 5) clearInterval(interval);
}, 1000);
```

#### Options:
A) Logs `1` to `5` every second.  
B) Logs `0` to `5` every second.  
C) Logs `5` infinitely every second.  
D) Does not log anything.

#### Answer:
A) Logs `1` to `5` every second.

---

### Question 5: **What is the output of the following string manipulation code?**
#### Code:
```javascript
const str = "  hello   world  ";
const trimmedStr = str.trim().replace(/\s+/g, '-');
console.log(trimmedStr);
```

#### Options:
A) `hello-world`  
B) `hello-world-`  
C) `hello world`  
D) `hello- world`

#### Answer:
A) `hello-world`

---

### Question 6: **What is the output of the following code using `JSON.stringify`?**
#### Code:
```javascript
const obj = { x: undefined, y: null, z: 10 };
console.log(JSON.stringify(obj));
```

#### Options:
A) `{"x":undefined,"y":null,"z":10}`  
B) `{"y":null,"z":10}`  
C) `{"x":null,"y":null,"z":10}`  
D) `{"x":undefined,"y":null}`

#### Answer:
B) `{"y":null,"z":10}`

---

### Question 7: **What will the following code with `Math.max` and `Math.min` return?**
#### Code:
```javascript
const values = [3, 1, 4, 1, 5, 9, 2, 6];
const max = Math.max(...values);
const min = Math.min(...values);
console.log(max, min);
```

#### Options:
A) `9 1`  
B) `6 1`  
C) `5 3`  
D) `9 2`

#### Answer:
A) `9 1`

---

### Question 8: **What will the following `forEach` loop output?**
#### Code:
```javascript
const array = [1, 2, 3];
array.forEach((value, index) => {
  console.log(index, value);
});
```

#### Options:
A) `1 2 3`  
B) `0 1`, `1 2`, `2 3`  
C) `1 2`, `2 3`, `3 4`  
D) `0 1`, `1 2`, `2 3`, `3 4`

#### Answer:
B) `0 1`, `1 2`, `2 3`

---

### Question 9: **What will this code output involving class inheritance?**
#### Code:
```javascript
class Car {
  constructor(model) {
    this.model = model;
  }
  start() {
    console.log(`${this.model} started.`);
  }
}

class ElectricCar extends Car {
  constructor(model, batteryLife) {
    super(model);
    this.batteryLife = batteryLife;
  }
  start() {
    console.log(`${this.model} started silently.`);
  }
}

const tesla = new ElectricCar('Tesla', '100 miles');
tesla.start();
```

#### Options:
A) `Tesla started.`  
B) `Tesla started silently.`  
C) `ElectricCar started.`  
D) `Car started silently.`

#### Answer:
B) `Tesla started silently.`

---

### Question 10: **What is the result of the following array filtering operation?**
#### Code:
```javascript
const arr = [1, 2, 3, 4, 5];
const evenNumbers = arr.filter(num => num % 2 === 0);
console.log(evenNumbers);
```

#### Options:
A) `[1, 3, 5]`  
B) `[2, 4]`  
C) `[1, 2, 3, 4, 5]`  
D) `[]`

#### Answer:
B) `[2, 4]`

---

### Question 11: **What will the following code using `map()` output?**
#### Code:
```javascript
const numbers = [1, 2, 3];
const doubled = numbers.map(num => num * 2);
console.log(doubled);
```

#### Options:
A) `[2, 4, 6]`  
B) `[1, 2, 3]`  
C) `[2, 3, 4]`  
D) `[1, 4, 9]`

#### Answer:
A) `[2, 4, 6]`

---

### Question 12: **What is the output of this code with `setTimeout`?**
#### Code:
```javascript
console.log('Start');
setTimeout(() => console.log('Delayed'), 2000);
console.log('End');
```

#### Options:
A) `Start End Delayed`  
B) `Start Delayed End`  
C) `Delayed Start End`  
D) `Start Delayed`

#### Answer:
A) `Start End Delayed`

---

### Question 13: **What does the following code using `Date` methods do?**
#### Code:
```javascript
const date = new Date();
date.setFullYear(date.getFullYear() + 2);
console.log(date.getFullYear());
```

#### Options:
A) Adds 2 years to the current year and outputs the updated year.  
B) Subtracts 2 years from the current year.  
C) Outputs the current year.  
D) Outputs the same date without changing the year.

#### Answer:
A) Adds 2 years to the current year and outputs the updated year.

---

### Question 14: **What does the `reduce` function do in this code?**
#### Code:
```javascript
const numbers = [1, 2, 3, 4];
const sum = numbers.reduce((acc, num) => acc + num, 0);
console.log(sum);
```

#### Options:
A) Multiplies all numbers together.  
B) Adds all numbers together.  
C) Returns the last element in the array.  
D) Filters out all numbers greater than 2.

#### Answer:
B) Adds all numbers together.

---

### Question 15: **What is the result of the following code involving `parseInt`?**
#### Code:
```javascript
const str = '10px';
const number = parseInt(str, 10);
console.log(number);
```

#### Options:
A) `NaN`  
B) `10`  
C) `0`  
D) `10px`

#### Answer:
B) `10`

---

### Question 16: **What will this code output with `setInterval`?**
#### Code:
```javascript
let i = 0;
const interval = setInterval(() => {
  i++;
  if (i > 5) clearInterval(interval);
  console.log(i);
}, 500);
```

#### Options:
A) Logs `1` to `5` every 0.5 seconds.  
B) Logs `1` to `5` every second.  
C) Logs `0` to `5` every second.  
D) Logs `0` to `10` every 0.5 seconds.

#### Answer:
A) Logs `1` to `5` every 0.5 seconds.

---

### Question 17: **What will the following code using `String.split` output?**
#### Code:
```javascript
const sentence = "The quick brown fox";
const words = sentence.split(" ");
console.log(words);
```

#### Options:
A) `["The", "quick", "brown", "fox"]`  
B) `["The quick", "brown fox"]`  
C) `["The", "quick brown fox"]`  
D) `["Thequickbrownfox"]`

#### Answer:
A) `["The", "quick", "brown", "fox"]`

---

### Question 18: **What is the result of the following code involving a `Date` object?**
#### Code:
```javascript
const date = new Date(2025, 2, 15);
console.log(date.getMonth());
```

#### Options:
A) `2`  
B) `3`  
C) `1`  
D) `0`

#### Answer:
A) `2` (since months are zero-indexed)

---

### Question 19: **What is the output of the following code using `JSON.parse` and `JSON.stringify`?**
#### Code:
```javascript
const jsonString = '{"name":"Alice","age":25}';
const parsedObject = JSON.parse(jsonString);
const stringifiedObject = JSON.stringify(parsedObject);
console.log(stringifiedObject);
```

#### Options:
A) `{"name":"Alice","age":25}`  
B) `{"name":"Alice", "age":25}`  
C) `"name":"Alice","age":25`  
D) `Alice,25`

#### Answer:
A) `{"name":"Alice","age":25}`

---

### Question 20: **What does the following code using `Math.pow` do?**
#### Code:
```javascript
const result = Math.pow(2, 3);
console.log(result);
```

#### Options:
A) `6`  
B) `8`  
C) `4`  
D) `2`

#### Answer:
B) `8`
