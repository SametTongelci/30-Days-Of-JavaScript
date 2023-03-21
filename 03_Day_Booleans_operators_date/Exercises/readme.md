## 💻 Day 3: Exercises and Solutions

### Exercises: Level 1

1. Declare firstName, lastName, country, city, age, isMarried, year variable and assign value to it and use the typeof operator to check different data types.

```js
let firstName = "Samet",
  lastName = "Töngelci",
  country = "Turkey",
  age = 25,
  isMarried = false,
  year = 2023;
console.log(typeof firstName); // string
console.log(typeof age); // number
console.log(typeof isMarried); // boolean
```

2. Check if type of '10' is equal to 10

```js
console.log(typeof "10" == typeof 10); // false
```

3. Check if parseInt('9.8') is equal to 10

```js
console.log(parseInt("9.8") == 10); // false
```

4. Boolean value is either true or false.

   1. Write three JavaScript statement which provide truthy value.

   ```js
   let truthy1 = true;
   let truthy2 = 5;
   let truthy3 = "true";
   ```

   2. Write three JavaScript statement which provide falsy value.

   ```js
   let falsy1 = 0;
   let falsy2 = null;
   let falsy3 = "";
   ```

5. Figure out the result of the following comparison expression first without using console.log(). After you decide the result confirm it using console.log()

   1. 4 > 3
   2. 4 >= 3
   3. 4 < 3
   4. 4 <= 3
   5. 4 == 4
   6. 4 === 4
   7. 4 != 4
   8. 4 !== 4
   9. 4 != '4'
   10. 4 == '4'
   11. 4 === '4'
   12. Find the length of python and jargon and make a falsy comparison statement.

   ```js
   console.log(4 > 3); // true
   console.log(4 >= 3); // true
   console.log(4 < 3); // false
   console.log(4 <= 3); // false
   console.log(4 == 4); // true
   console.log(4 === 4); // true
   console.log(4 != 4); // false
   console.log(4 !== 4); // false
   console.log(4 != "4"); // false
   console.log(4 !== "4"); // true
   console.log(4 == "4"); // true
   console.log(4 === "4"); // false
   console.log("python".length !== "jargon".length); // false
   ```

6. Figure out the result of the following expressions first without using console.log(). After you decide the result confirm it by using console.log()

   1. 4 > 3 && 10 < 12
   2. 4 > 3 && 10 > 12
   3. 4 > 3 || 10 < 12
   4. 4 > 3 || 10 > 12
   5. !(4 > 3)
   6. !(4 < 3)
   7. !(false)
   8. !(4 > 3 && 10 < 12)
   9. !(4 > 3 && 10 > 12)
   10. !(4 === '4')
   11. There is no 'on' in both dragon and python

   ```js
   console.log(4 > 3 && 10 < 12); // true
   console.log(4 > 3 && 10 > 12); // false
   console.log(4 > 3 || 10 < 12); // true
   console.log(4 > 3 || 10 > 12); // true
   console.log(!(4 > 3)); //false
   console.log(!(4 < 3)); // true
   console.log(!false); // true
   console.log(!(4 > 3 && 10 < 12)); // false
   console.log(!(4 > 3 && 10 > 12)); // true
   console.log(!(4 === "4")); // true
   console.log(!("python".includes("on") && "dragon".includes("on"))); // false
   ```

7. Use the Date object to do the following activities
   1. What is the year today?
   2. What is the month today as a number?
   3. What is the date today?
   4. What is the day today as a number?
   5. What is the hours now?
   6. What is the minutes now?
   7. Find out the numbers of seconds elapsed from January 1, 1970 to now.
   ```js
   const now = new Date();
   console.log(now.getFullYear());
   console.log(now.getMonth());
   console.log(now.getDate());
   console.log(now.getDay());
   console.log(now.getHours());
   console.log(now.getMinutes());
   console.log(now.getTime());
   ```

### Exercises: Level 2

1. Write a script that prompt the user to enter base and height of the triangle and calculate an area of a triangle (area = 0.5 x b x h).

   ```sh
   Enter base: 20
   Enter height: 10
   The area of the triangle is 100
   ```

   ```js
   let base = prompt("Enter base of triangle: ");
   let height = prompt("Enter height of triangle: ");
   console.log(
     "The area of the triangle is",
     (parseFloat(base) * parseFloat(height)) / 2
   );
   ```

2. Write a script that prompt the user to enter side a, side b, and side c of the triangle and and calculate the perimeter of triangle (perimeter = a + b + c)

   ```sh
   Enter side a: 5
   Enter side b: 4
   Enter side c: 3
   The perimeter of the triangle is 12
   ```

   ```js
   let sideA = prompt("Enter side a of triangle: ");
   let sideB = prompt("Enter side b of triangle: ");
   let sideC = prompt("Enter side c of triangle: ");
   console.log(
     "The perimeter of the triangle is",
     parseFloat(sideA) + parseFloat(sideB) + parseFloat(sideC)
   );
   ```

3. Get length and width using prompt and calculate an area of rectangle (area = length x width and the perimeter of rectangle (perimeter = 2 x (length + width))

   ```js
   let length = Number(prompt("Enter length of rectangle: "));
   let width = Number(prompt("Enter width of rectangle: "));
   console.log("The area of the rectangle is", length * width);
   console.log("The perimeter of the rectangle is", 2 * (length + width));
   ```

4. Get radius using prompt and calculate the area of a circle (area = pi x r x r) and circumference of a circle(c = 2 x pi x r) where pi = 3.14.

   ```js
   let radius = parseFloat(prompt("Enter radius of circle: "));
   let pi = 3.14;
   console.log("The area of the circle:", pi * radius ** 2);
   console.log("The circumference of the circle:", 2 * pi * radius);
   ```

5. Calculate the slope, x-intercept and y-intercept of y = 2x -2

   ```js
   let a = 1,
     b = 2,
     c = -2;
   console.log(
     "x_intercept:",
     -c / b,
     "y_intercept:",
     c / a,
     "slope of the y = 2x -2 is :",
     b
   );
   ```

6. Slope is m = (y<sub>2</sub>-y<sub>1</sub>)/(x<sub>2</sub>-x<sub>1</sub>). Find the slope between point (2, 2) and point(6,10)

   ```js
   let slope = (10 - 2) / (6 - 2);
   console.log(slope);
   ```

7. Compare the slope of above two questions.

   ```js
   console.log(b === slope); /// true
   ```

8. Calculate the value of y (y = x<sup>2</sup> + 6x + 9). Try to use different x values and figure out at what x value y is 0.

   ```js
   let a = 1;   // coefficient of x^2
   let b = 6;   // coefficient of x
   let c = 9;   // constant
   let discriminant = b**2 - (4 * a * c);   // 0
   let root1 = (-b + Math.sqrt(discriminant)) / (2 * a)  // -3
   let root2 = (-b - Math.sqrt(discriminant)) / (2 * a)  // -3
   root1 === root2 ? console.log('x: 'root1) : console.log('x:', root1, 'or x :', root2);  // y = 0 for x = -3
   ```

9. Writ a script that prompt a user to enter hours and rate per hour. Calculate pay of the person?

   ```sh
   Enter hours: 40
   Enter rate per hour: 28
   Your weekly earning is 1120
   ```

   ```js
   let hours = parseFloat(prompt("Enter hours:"));
   let rate = parseFloat(prompt("Enter rate per hour:"));
   console.log("Your weekly earning is:", hours * rate);
   ```

10. If the length of your name is greater than 7 say, your name is long else say your name is short.

```js
let name = prompt("Enter your name:");
name.length > 7
  ? console.log("Your name is long")
  : console.log("Your name is short");
```

11. Compare your first name length and your family name length and you should get this output.

```js
let firstName = "Asabeneh";
let lastName = "Yetayeh";
```

```sh
Your first name, Asabeneh is longer than your family name, Yetayeh
```

```js
let firstName = "Samet";
let lastName = "Töngelci";
firstName.length > lastName.length
  ? console.log(
      `Your first name ${firstName} is longer than your family name, ${lastName}`
    )
  : console.log(
      `Your first name ${firstName} is shorter than your family name, ${lastName}`
    );
```

12. Declare two variables _myAge_ and _yourAge_ and assign them initial values and myAge and yourAge.

```js
let myAge = 250;
let yourAge = 25;
```

```sh
I am 225 years older than you.
```

```js
let myAge = 250,
  yourAge = 25;
myAge > yourAge
  ? console.log(`I am ${myAge - yourAge} years older than you.`)
  : console.log(`You are ${yourAge - myAge} years older than me.`);
```

13. Using prompt get the year the user was born and if the user is 18 or above allow the user to drive if not tell the user to wait a certain amount of years.

```sh

Enter birth year: 1995
You are 25. You are old enough to drive

Enter birth year: 2005
You are 15. You will be allowed to drive after 3 years.
```

```js
let birthYear = parseInt(prompt("Enter your birth year:"));
let age = new Date().getFullYear() - birthYear;
age >= 18
  ? console.log(`You are ${age}. You are old enough to drive.`)
  : console.log(
      `You are ${age}. You will be allowed to drive after ${18 - age} years.`
    );
```

14. Write a script that prompt the user to enter number of years. Calculate the number of seconds a person can live. Assume some one lives just hundred years

```sh
Enter number of years you live: 100
You lived 3153600000 seconds.
```

```js
let age = parseInt(prompt("Enter your age: "));
let remainingYears = 100 - age;
let remainingSeconds = remainingYears * 365 * 24 * 60 * 60;
console.log(
  `You have lived ${
    age * 365 * 24 * 60 * 60
  } seconds. You have ${remainingSeconds} seconds more to live reach 100 years.`
);
```

15. Create a human readable time format using the Date time object
    i. YYYY-MM-DD HH:mm
    ii. DD-MM-YYYY HH:mm
    iii. DD/MM/YYYY HH:mm

```js
let info = new Date(),
  year = info.getFullYear(),
  month = info.getMonth(),
  date = info.getDate(),
  hours = info.getHours(),
  minutes = info.getMinutes();
console.log(`i. ${year}-${month}-${date} ${hours}:${minutes}`);
console.log(`ii. ${date}-${month}-${year} ${hours}:${minutes}`);
console.log(`iii. ${date}/${month}/${year} ${hours}:${minutes}`);
```

### Exercises: Level 3

1. Create a human readable time format using the Date time object. The hour and the minute should be all the time two digits(7 hours should be 07 and 5 minutes should be 05 )
   i. YYY-MM-DD HH:mm eg. 20120-01-02 07:05

```js
let info = new Date(),
  year = info.getFullYear(),
  month = info.getMonth(),
  date = info.getDate(),
  hours = info.getHours(),
  minutes = info.getMinutes();
month < 10 ? (month = `0${month}`) : (month = month);
date < 10 ? (date = `0${date}`) : (date = date);
hours < 10 ? (hours = `0${hours}`) : (hours = hours);
minutes < 10 ? (minutes = `0${minutes}`) : (minutes = minutes);
console.log(`${year}-${month}-${date} ${hours}:${minutes}`);
```
