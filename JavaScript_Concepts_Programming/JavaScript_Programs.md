# JavaScript Programs

This repository contains various JavaScript programs demonstrating different concepts and logic implementations.

## File Structure
```
JS_Programs/
  ├── even-odd-count.js
  ├── number-sequence.js
  ├── star-pattern.js
  ├── identity-matrix.js
  ├── student-results.js
```

## Programs

### 1. Even and Odd Count (`even-odd-count.js`)
```javascript
let numbers= [50, 65, 56, 71, 81, 33];
let evencount=0;
let oddcount=0;
for (i=0; i < numbers.length; i++)
{
    if (numbers[i] % 2 === 0)
    {
    evencount +=1;
    
    } 
    
    else
    {
    oddcount +=1;
    
    }
}
    console.log(`Even Count: ${evencount} odd Count: ${oddcount}`);
```
![Even and Odd Count](https://github.com/AniketP117/BootStrap_Project-JavaScript_Concepts/blob/27ae5863fd31c70f40abe9228b5e0aeecd05be44/Images/JS_Images/Even%20and%20Odd%20Count%20Output.png)

### 2. Number Sequence (`number-sequence.js`)
```javascript
const readline = require('readline');

const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout
});

rl.question('Enter a number: ', (num) => {
  for (let i = 1; i < num; i += 2) {
    console.log(i);
  }
  rl.close();
});
```
![Number Sequence](https://github.com/AniketP117/BootStrap_Project-JavaScript_Concepts/blob/27ae5863fd31c70f40abe9228b5e0aeecd05be44/Images/JS_Images/Number%20Sequence%20Output.png)


### 3. Star Pattern (`star-pattern.js`)
```javascript
for (let i = 1; i <= 9; i++) {
    let stars = "";
    for (let j = 1; j <= 9; j++) {
      if (j <= i) {
        stars += "*";
      } else {
        stars += " ";
      }
    }
    console.log(stars);
  }
```

![Star Pattern](https://github.com/AniketP117/BootStrap_Project-JavaScript_Concepts/blob/27ae5863fd31c70f40abe9228b5e0aeecd05be44/Images/JS_Images/Number%20Sequence%20Output.png)

### 4. Identity Matrix (`identity-matrix.js`)
```javascript
function createMatrix(n) {
    let matrix = [];
  
    for (let i = 0; i < n; i++) {
      let row = [];
      for (let j = 0; j < n; j++) {
        row.push(i === j ? 1 : 0); 
      }
      matrix.push(row);
    }
  
   
    for (let i = 0; i < n; i++) {
      console.log(matrix[i].join(" "));
    }
  }
  
 
  createMatrix(3);
```
![Identity Matrix](https://github.com/AniketP117/BootStrap_Project-JavaScript_Concepts/blob/27ae5863fd31c70f40abe9228b5e0aeecd05be44/Images/JS_Images/Identity%20Matrix%20Output.png)

### 5. Student Results (`student-results.js`)
```javascript
let students = [
    { rollNumber: 111, marks: 81 },
    { rollNumber: 222, marks: 75 },
    { rollNumber: 333, marks: 43 },
    { rollNumber: 444, marks: 58 }
];

function Result(marks) {
    if (marks > 79) {
        return "Honors";
    } else if (marks >= 50 && marks <= 79) {
        return "1st Division";
    } else {
        return "Fail";
    }
}

students.forEach(student => {
    console.log(`Roll Number: ${student.rollNumber}, Marks: ${student.marks}, Result: ${Result(student.marks)}`);
});
```
![Student Results](https://github.com/AniketP117/BootStrap_Project-JavaScript_Concepts/blob/27ae5863fd31c70f40abe9228b5e0aeecd05be44/Images/JS_Images/Student%20Results%20Output.png)


## Usage
Clone the repository and run each file using Node.js:
```bash
node <filename.js>
```

## Future Enhancements
- Add more complex algorithms and data structure implementations.
- Improve user input handling and validation.
- Implement interactive web-based versions of these programs.
- Optimize performance for large-scale computations.
- Include test cases for better reliability.
