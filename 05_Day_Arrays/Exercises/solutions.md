# Day-5 Exercises & Solutions

### Exercise: Level 1

```js
const countries = [
  "Albania",
  "Bolivia",
  "Canada",
  "Denmark",
  "Ethiopia",
  "Finland",
  "Germany",
  "Hungary",
  "Ireland",
  "Japan",
  "Kenya",
];

const webTechs = [
  "HTML",
  "CSS",
  "JavaScript",
  "React",
  "Redux",
  "Node",
  "MongoDB",
];
```

1. Declare an _empty_ array;

```js
let empty_array = [];
```

2. Declare an array with more than 5 number of elements

```js
let array = [1, 2, "a", null, "name", 50, true];
```

3. Find the length of your array

```js
console.log(array.length); // 7
```

4. Get the first item, the middle item and the last item of the array

```js
console.log(array[0], array[(array.length - 1) / 2], array[array.length - 1]);
```

5. Declare an array called _mixedDataTypes_, put different data types in the array and find the length of the array. The array size should be greater than 5

```js
let mixedDataTypes = [
  "firstName",
  0,
  "arr",
  null,
  13,
  false,
  "true",
  undefined,
];
console.log(mixedDataTypes.length);
```

6. Declare an array variable name itCompanies and assign initial values Facebook, Google, Microsoft, Apple, IBM, Oracle and Amazon

```js
let itCompanies = [
  "Facebook",
  "Google",
  "Microsoft",
  "Apple",
  "IBM",
  "Oracle",
  "Amazon",
];
```

7. Print the array using _console.log()_

```js
console.log(itCompanies);
```

8. Print the number of companies in the array

```js
console.log(itCompanies.length);
```

9. Print the first company, middle and last company

```js
console.log(
  itCompanies[0],
  itCompanies[(itCompanies.length - 1) / 2],
  itCompanies[itCompanies.length - 1]
);
```

10. Print out each company

```js
itCompanies.forEach(function (item) {
  console.log(item);
});
```

11. Change each company name to uppercase one by one and print them out

```js
let upperCase = itCompanies.map((element) => element.toUpperCase());
console.log(upperCase);
```

12. Print the array like as a sentence: Facebook, Google, Microsoft, Apple, IBM,Oracle and Amazon are big IT companies.

```js
console.log(itCompanies.join(", ") + " are big IT companies.");
```

13. Check if a certain company exists in the itCompanies array. If it exist return the company else return a company is _not found_

```js
let index = itCompanies.includes("Amazon");
if (index === false) {
  console.log("not found");
} else {
  console.log("Amazon");
}
```

14. Filter out companies which have more than one 'o' without the filter method

```js
let moreThanOne = [];
itCompanies.forEach(function (item) {
  if (
    item.indexOf("o") !== -1 &&
    item.lastIndexOf("o") !== -1 &&
    item.indexOf("o") !== item.lastIndexOf("o")
  ) {
    moreThanOne.push(item);
  }
});
console.log(moreThanOne);
```

15. Sort the array using _sort()_ method

```js
console.log(itCompanies.sort());
```

16. Reverse the array using _reverse()_ method

```js
console.log(itCompanies.reverse());
```

17. Slice out the first 3 companies from the array

```js
console.log(itCompanies.slice(0, 3));
```

18. Slice out the last 3 companies from the array

```js
console.log(itCompanies.slice(itCompanies.length - 3));
```

19. Slice out the middle IT company or companies from the array

```js
let itCompanies = [
  "Facebook",
  "Google",
  "Microsoft",
  "Apple",
  "IBM",
  "Oracle",
  "Amazon",
];
itCompanies.sort();
let middle = itCompanies.slice(
  (itCompanies.length - 1) / 2,
  (itCompanies.length - 1) / 2 + 1
);
console.log(middle);
```

20. Remove the first IT company from the array

```js
console.log(itCompanies.splice(0, 1));
```

21. Remove the middle IT company or companies from the array

```js
if (itCompanies.length % 2 === 0) {
  console.log(itCompanies.splice(itCompanies.length / 2 - 1, 2));
} else {
  console.log(itCompanies.splice((itCompanies.length - 1) / 2, 1));
}
```

22. Remove the last IT company from the array

```js
console.log(itCompanies.splice(itCompanies.length - 1, 1));
```

23. Remove all IT companies

```js
console.log(itCompanies.splice(0, itCompanies.length));
```

### Exercise: Level 2

1. Create a separate countries.js file and store the countries array in to this file, create a separate file web_techs.js and store the webTechs array in to this file. Access both file in main.js file

```
You can see the solution in main.js, country.js and web_techs.js files
```

2. First remove all the punctuations and change the string to array and count the number of words in the array

   ```js
   let text =
     "I love teaching and empowering people. I teach HTML, CSS, JS, React, Python.";
   console.log(words);
   console.log(words.length);
   ```

   ```sh
   ["I", "love", "teaching", "and", "empowering", "people", "I", "teach", "HTML", "CSS", "JS", "React", "Python"]

   13
   ```

```js
let newText = text.replace(/[^a-zA-Z ]/g, "");
array = newText.split(" ");
console.log(array.length);
```

3.  In the following shopping cart add, remove, edit items

    ```js
    const shoppingCart = ["Milk", "Coffee", "Tea", "Honey"];
    ```

    - add 'Meat' in the beginning of your shopping cart if it has not been already added`

    ```js
    if (shoppingCart.includes("Meat") === false) {
      shoppingCart.unshift("Meat");
    }
    ```

    - add Sugar at the end of you shopping cart if it has not been already added

    ```js
    if (shoppingCart.includes("Sugar") === false) {
      shoppingCart.push("Sugar");
    }
    ```

    - remove 'Honey' if you are allergic to honey

      ```js
      if (shoppingCart.indexOf("Honey") !== -1) {
        shoppingCart.splice(shoppingCart.indexOf("Honey"), 1);
      }
      ```

    - modify Tea to 'Green Tea'

      ```js
      if (shoppingCart.indexOf("Tea") !== -1) {
        shoppingCart[shoppingCart.indexOf("Tea")] = "Green Tea";
      }
      ```

4.  In countries array check if 'Ethiopia' exists in the array if it exists print 'ETHIOPIA'. If it does not exist add to the countries list.

    ```js
    const countries = [
      "Albania",
      "Bolivia",
      "Canada",
      "Denmark",
      "Ethiopia",
      "Finland",
      "Germany",
      "Hungary",
      "Ireland",
      "Japan",
      "Kenya",
    ];
    if (countries.includes("Ethiopia") !== false) {
      console.log("ETHIOPIA");
    } else {
      countries.push("Ethiopia");
    }
    ```

5.  In the webTechs array check if Sass exists in the array and if it exists print 'Sass is a CSS preprocess'. If it does not exist add Sass to the array and print the array.

    ```js
    const webTechs = [
      "HTML",
      "CSS",
      "JavaScript",
      "React",
      "Redux",
      "Node",
      "MongoDB",
    ];
    if (webTechs.includes("Sass") !== false) {
      console.log("Sass is a CSS preprocess");
    } else {
      webTechs.push("Sass");
      console.log(webTechs);
    }
    ```

6.  Concatenate the following two variables and store it in a fullStack variable.

    ```js
    const frontEnd = ["HTML", "CSS", "JS", "React", "Redux"];
    const backEnd = ["Node", "Express", "MongoDB"];

    console.log(fullStack);
    ```

    ```sh
    ["HTML", "CSS", "JS", "React", "Redux", "Node", "Express", "MongoDB"]
    ```

```js
const fullStack = frontEnd.concat(backEnd);
console.log(fullStack);
```

### Exercise: Level 3

1.  The following is an array of 10 students ages:

        ```js
        const ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24]
        ```

        - Sort the array and find the min and max age
        - Find the median age(one middle item or two middle items divided by two)
        - Find the average age(all items divided by number of items)
        - Find the range of the ages(max minus min)
        - Compare the value of (min - average) and (max - average), use _abs()_ method

    1.Slice the first ten countries from the [countries array](https://github.com/Asabeneh/30DaysOfJavaScript/tree/master/data/countries.js)

1.  Find the middle country(ies) in the [countries array](https://github.com/Asabeneh/30DaysOfJavaScript/tree/master/data/countries.js)
1.  Divide the countries array into two equal arrays if it is even. If countries array is not even , one more country for the first half.
