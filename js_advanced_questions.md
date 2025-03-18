
### Question 1: What will the following code snippet output?
#### Code:
```javascript
class Animal {
  constructor(name, type) {
    this.name = name;
    this.type = type;
  }

  getInfo() {
    return `${this.name} is a ${this.type}.`;
  }

  static getSpecies() {
    return 'Animal';
  }
}

class Dog extends Animal {
  constructor(name, breed) {
    super(name, 'Dog');
    this.breed = breed;
  }

  getBreed() {
    return `The breed of ${this.name} is ${this.breed}.`;
  }
}

const myDog = new Dog('Buddy', 'Golden Retriever');
console.log(myDog.getInfo());
console.log(myDog.getBreed());
console.log(Dog.getSpecies());
```

#### Options:
A) Buddy is a Dog. The breed of Buddy is Golden Retriever. Animal  
B) Buddy is a Dog. The breed of Buddy is Golden Retriever. Dog  
C) The breed of Buddy is Golden Retriever. Animal  
D) Animal. Buddy is a Dog. The breed of Buddy is Golden Retriever.

#### Answer:
A) Buddy is a Dog. The breed of Buddy is Golden Retriever. Animal

---

### Question 2: What is the output of the following code that involves string manipulation?
#### Code:
```javascript
function reverseString(str) {
  let reversed = '';
  for (let i = str.length - 1; i >= 0; i--) {
    reversed += str[i];
  }
  return reversed;
}

const str = "Hello, World!";
const reversedStr = reverseString(str);
console.log(reversedStr);
```

#### Options:
A) !dlroW ,olleH  
B) Hello, World!  
C) HelloWorld  
D) dlroW ,olleH!

#### Answer:
A) !dlroW ,olleH

---

### Question 3: What will the following asynchronous JavaScript code output?
#### Code:
```javascript
const asyncExample = async () => {
  let result = 'start';
  try {
    const promise = new Promise((resolve, reject) => {
      setTimeout(() => resolve('done'), 1000);
    });
    result = await promise;
  } catch (error) {
    result = 'error';
  }
  return result;
};

asyncExample().then(data => console.log(data));
```

#### Options:
A) start  
B) done  
C) error  
D) undefined

#### Answer:
B) done

---

### Question 4: What will be the result of the following code involving JSON?
#### Code:
```javascript
const person = {
  name: "John",
  age: 30,
  city: "New York"
};

const jsonString = JSON.stringify(person);
console.log(jsonString);
```

#### Options:
A) { name: "John", age: 30, city: "New York" }  
B) "{"name":"John","age":30,"city":"New York"}"  
C) {"name":"John","age":30,"city":"New York"}  
D) {"name": "John", "age": 30, "city": "New York"}

#### Answer:
B) "{"name":"John","age":30,"city":"New York"}"

---

### Question 5: Which of the following will display an alert when a form input is empty?
#### Code:
```html
<form id="myForm">
  <label for="name">Name:</label>
  <input type="text" id="name" name="name">
  <input type="submit" value="Submit">
</form>

<script>
  document.getElementById('myForm').addEventListener('submit', function(event) {
    const name = document.getElementById('name').value;
    if (!name) {
      event.preventDefault();
      alert('Name is required!');
    }
  });
</script>
```

#### Options:
A) The form will be submitted even if the name field is empty.  
B) The form will not be submitted and an alert will show: "Name is required!".  
C) The form will be submitted without validation.  
D) The alert will show "Name is valid!".

#### Answer:
B) The form will not be submitted and an alert will show: "Name is required!".

---

### Question 6: What is the result of the following code that involves a Timer function and Async/Await?
#### Code:
```javascript
async function delay(ms) {
  return new Promise(resolve => setTimeout(resolve, ms));
}

async function execute() {
  console.log('Start');
  await delay(2000);
  console.log('End');
}

execute();
```

#### Options:
A) Start End (after 2 seconds)  
B) Start End (immediately)  
C) End Start  
D) No output

#### Answer:
A) Start End (after 2 seconds)

---

### Question 7: What is the output of the following code involving date manipulation?
#### Code:
```javascript
const date = new Date('2025-03-20');
const nextWeek = new Date(date);
nextWeek.setDate(date.getDate() + 7);
console.log(nextWeek.toDateString());
```

#### Options:
A) Mon Mar 27 2025  
B) Fri Mar 27 2025  
C) Sun Mar 27 2025  
D) Wed Mar 27 2025

#### Answer:
B) Fri Mar 27 2025

---

### Question 8: What will the following code produce when using media queries in CSS?
#### Code:
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      font-size: 16px;
    }
    @media (max-width: 600px) {
      body {
        font-size: 12px;
      }
    }
  </style>
</head>
<body>
  <p>Hello, world!</p>
</body>
</html>
```

#### Options:
A) The font size will be 16px on any screen size.  
B) The font size will be 12px on screens smaller than 600px width.  
C) The font size will always be 16px, regardless of screen size.  
D) There is no change in the font size.

#### Answer:
B) The font size will be 12px on screens smaller than 600px width.

---

### Question 9: What will the following JavaScript code output when used for pagination?
#### Code:
```javascript
const data = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
const pageSize = 3;

function paginate(arr, pageSize) {
  const pages = [];
  for (let i = 0; i < arr.length; i += pageSize) {
    pages.push(arr.slice(i, i + pageSize));
  }
  return pages;
}

console.log(paginate(data, pageSize));
```

#### Options:
A) [[1, 2, 3], [4, 5, 6], [7, 8, 9], [10]]  
B) [[1, 2], [3, 4], [5, 6], [7, 8], [9, 10]]  
C) [[1, 2, 3, 4], [5, 6, 7, 8], [9, 10]]  
D) [[1, 2, 3, 4, 5], [6, 7, 8, 9], [10]]

#### Answer:
A) [[1, 2, 3], [4, 5, 6], [7, 8, 9], [10]]

---

### Question 10: What will the following code involving animation in JavaScript output?
#### Code:
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    @keyframes move {
      from {
        transform: translateX(0);
      }
      to {
        transform: translateX(100px);
      }
    }

    .animated {
      width: 100px;
      height: 100px;
      background-color: red;
      animation: move 2s infinite alternate;
    }
  </style>
</head>
<body>
  <div class="animated"></div>
</body>
</html>
```

#### Options:
A) The red square will move 100px to the right and then back to the left repeatedly.  
B) The red square will rotate continuously.  
C) The red square will grow in size continuously.  
D) There is no animation effect.

#### Answer:
A) The red square will move 100px to the right and then back to the left repeatedly.
