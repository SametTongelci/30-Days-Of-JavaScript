## 💻 Day 4: Exercises & Solutions

### Exercises: Level 1

1. Get user input using prompt(“Enter your age:”). If user is 18 or older , give feedback:'You are old enough to drive' but if not 18 give another feedback stating to wait for the number of years he needs to turn 18.

   ```sh
   Enter your age: 30
   You are old enough to drive.

   Enter your age:15
   You are left with 3 years to drive.
   ```

   ```js
   let age = parseInt(prompt("Enter your age: "));
   age >= 18
     ? console.log("You are old enough to drive.")
     : console.log(`Yo are left with ${18 - age} years to drive.`);
   ```

1. Compare the values of myAge and yourAge using if … else. Based on the comparison and log the result to console stating who is older (me or you). Use prompt(“Enter your age:”) to get the age as input.

   ```sh
   Enter your age: 30
   You are 5 years older than me.
   ```

   ```js
   let myAge = 25;
   let yourAge = parseInt(prompt("Enter your age: "));
   if (myAge > yourAge) {
     console.log(`I am ${myAge - yourAge} years older than you.`);
   } else if (yourAge > myAge) {
     console.log(`You are ${yourAge - myAge} years older than me.`);
   } else {
     console.log("We are the same age.");
   }
   ```

1. If a is greater than b return 'a is greater than b' else 'a is less than b'. Try to implement it in to ways

   - using if else
   - ternary operator.

   ```js
   let a = 4;
   let b = 3;
   ```

   ```sh
     4 is greater than 3
   ```

   ```js
   // Solution with if-else
   let a = 4;
   let b = 3;
   if (a > b) {
     console.log(`${a} is greater than ${b}`);
   } else {
     console.log(`${b} is greater than ${a}`);
   }
   // Solution with Ternary Operator
   a > b
     ? console.log(`${a} is greater than ${b}`)
     : console.log(`${b} is greater than ${a}`);
   ```

1. Even numbers are divisible by 2 and the remainder is zero. How do you check, if a number is even or not using JavaScript?

   ```sh
   Enter a number: 2
   2 is an even number

   Enter a number: 9
   9 is is an odd number.
   ```

   ```js
   let number = Number(prompt("Enter a number: "));
   number % 2 === 0
     ? console.log(number, "is a even nnumber")
     : console.log(number, "is an odd number.");
   ```

### Exercises: Level 2

1. Write a code which can give grades to students according to theirs scores:
   - 80-100, A
   - 70-89, B
   - 60-69, C
   - 50-59, D
   - 0-49, F
   ```js
   let grade = Number(prompt("Enter your grade: "));
   switch (true) {
     case grade >= 80 && grade <= 100:
       console.log("A");
       break;
     case grade >= 70 && grade < 80:
       console.log("B");
       break;
     case grade >= 60 && grade < 70:
       console.log("C");
       break;
     case grade >= 50 && grade < 60:
       console.log("D");
       break;
     case grade >= 0 && grade < 50:
       console.log("F");
       break;
     default:
       console.log("Enter your grade between 0 and 100");
   }
   ```
1. Check if the season is Autumn, Winter, Spring or Summer.
   If the user input is :
   - September, October or November, the season is Autumn.
   - December, January or February, the season is Winter.
   - March, April or May, the season is Spring
   - June, July or August, the season is Summer

```js
let month = prompt("What month are we in?");
switch (month) {
  case "September":
  case "October":
  case "November":
    console.log("The season is Autumn");
    break;
  case "December":
  case "January":
  case "February":
    console.log("The season is Winter");
    break;
  case "March":
  case "April":
  case "May":
    console.log("The season is Spring");
    break;
  case "June":
  case "July":
  case "August":
    console.log("The season is Summer");
    break;
  default:
    console.log("Enter a valid month name!");
    break;
}
```

1. Check if a day is weekend day or a working day. Your script will take day as an input.

```sh
    What is the day  today? Saturday
    Saturday is a weekend.

    What is the day today? saturDaY
    Saturday is a weekend.

    What is the day today? Friday
    Friday is a working day.

    What is the day today? FrIDAy
    Friday is a working day.
```

```js
let day = prompt("What is the day today?");
day = day.toLowerCase();
day = day.charAt(0).toUpperCase() + day.slice(1);
switch (day) {
  case "Monday":
  case "Tuesday":
  case day === "Wednesday":
  case "Thursday":
  case "Friday":
    console.log(day, "is a working day.");
    break;
  case "Saturday":
  case "Sunday":
    console.log(day, "is a weekend.");
    break;
  default:
    console.log("Enter a valid day...");
    break;
}
```

### Exercises: Level 3

1. Write a program which tells the number of days in a month.

```sh
  Enter a month: January
  January has 31 days.

  Enter a month: JANUARY
  January has 31 day

  Enter a month: February
  February has 28 days.

  Enter a month: FEbruary
  February has 28 days.
```

1. Write a program which tells the number of days in a month, now consider leap year.
