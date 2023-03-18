## 💻 Day 2: Exercises and Solutions

### Exercise: Level 1

1. Declare a variable named challenge and assign it to an initial value **'30 Days Of JavaScript'**.
```js
let challenge = '30 Days Of JavaScript'
```
2. Print the string on the browser console using __console.log()__
```js
console.log(challenge)
```
3. Print the __length__ of the string on the browser console using _console.log()_
```js
console.log(challenge.length)
```
4. Change all the string characters to capital letters using __toUpperCase()__ method
```js
console.log(challenge.toUpperCase())
```
5. Change all the string characters to lowercase letters using __toLowerCase()__ method
```js
console.log(challenge.toLowerCase())
```
6. Cut (slice) out the first word of the string using __substr()__ or __substring()__ method
```js
console.log(challenge.substr(0,2))
console.log(challenge.substring(0,2))
```
7. Slice out the phrase *Days Of JavaScript* from *30 Days Of JavaScript*.
```js
console.log(challenge.slice(3, challenge.length))
```
8. Check if the string contains a word __Script__ using __includes()__ method
```js
console.log(challenge.includes('Script'))
```
9. Split the __string__ into an __array__ using __split()__ method
```js
console.log(challenge.split(''))
```
10. Split the string 30 Days Of JavaScript at the space using __split()__ method
```js
console.log(challenge.split(' '))
```
11. 'Facebook, Google, Microsoft, Apple, IBM, Oracle, Amazon' __split__ the string at the comma and change it to an array.
```js
console.log('Facebook, Google, Microsoft, Apple, IBM, Oracle, Amazon'.split(','))
```
12. Change 30 Days Of JavaScript to 30 Days Of Python using __replace()__ method.
```js
console.log(challenge.replace('JavaScript', 'Python'))
```
13. What is character at index 15 in '30 Days Of JavaScript' string? Use __charAt()__ method.
```js
console.log(challenge.charAt(15))
```
14. What is the character code of J in '30 Days Of JavaScript' string using __charCodeAt()__
```js
console.log(challenge.charCodeAt('J'))
```
15. Use __indexOf__ to determine the position of the first occurrence of __a__ in 30 
Days Of JavaScript
```js
console.log(challenge.indexOf('a'))
```
16. Use __lastIndexOf__ to determine the position of the last occurrence of __a__ in 30 Days Of JavaScript.
```js
console.log(challenge.lastIndexOf('a'))
```
17. Use __indexOf__ to find the position of the first occurrence of the word __because__ in the following sentence:__'You cannot end a sentence with because because because is a conjunction'__
```js
console.log('You cannot end a sentence with because because because is a conjunction'.indexOf('because'))
```
18. Use __lastIndexOf__ to find the position of the last occurrence of the word __because__ in the following sentence:__'You cannot end a sentence with because because because is a conjunction'__
```js
console.log('You cannot end a sentence with because because because is a conjunction'.lastIndexOf('because'))
```
19. Use __search__ to find the position of the first occurrence of the word __because__ in the following sentence:__'You cannot end a sentence with because because because is a conjunction'__
```js
console.log('You cannot end a sentence with because because because is a conjunction'.search('because'))
```
20. Use __trim()__ to remove any trailing whitespace at the beginning and the end of a string.E.g ' 30 Days Of JavaScript '.
```js
console.log(' 30 Days Of JavaScript '.trim())
```
21. Use __startsWith()__ method with the string *30 Days Of JavaScript* and make the result true
```js
console.log(challenge.startsWith('30'))
```
22. Use __endsWith()__ method with the string *30 Days Of JavaScript* and make the result true
```js
console.log(challenge.endsWith('t'))
```
23. Use __match()__ method to find all the __a__’s in 30 Days Of JavaScript
```js
console.log(challenge.match(/a/gi))
```
24. Use __concat()__ and merge '30 Days of' and 'JavaScript' to a single string, '30 Days Of JavaScript'
```js
console.log('30 Days of '.concat('JavaScript'))
```
25. Use __repeat()__ method to print 30 Days Of JavaScript 2 times
```js
console.log(challenge.repeat(2))
```

### Exercise: Level 2

1. Using console.log() print out the following statement:
    ```sh
    The quote 'There is no exercise better for the heart than reaching down and lifting people up.' by John Holmes teaches us to help one another.
    ```
```js
console.log("The quote \'There is no exercise better for the heart than reaching down and lifting people up.\' by John Holmes teaches us to help one another.")
```
2. Using console.log() print out the following quote by Mother Teresa:
    ```sh
    "Love is not patronizing and charity isn't about pity, it is about love. Charity and love are the same -- with charity you give love, so don't just give money but reach out your hand instead."
    ```
```js
console.log('"Love is not patronizing and charity isn\'t about pity, it is about love. Charity and love are the same -- with charity you give love, so don\'t just give money but reach out your hand instead."')
```
3. Check if typeof '10' is exactly equal to 10. If not make it exactly equal.
```js
console.log('10' === 10) // false
console.log(parseFloat('10') === 10)  // true
```
4. Check if parseFloat('9.8') is equal to 10 if not make it exactly equal with 10.
```js
console.log(parseFloat('9.8') === 10)  // false
console.log(Math.round(parseFloat('9.8')) === 10)  // true
```
5. Check if 'on' is found in both python and jargon
```js
console.log('python'.includes('on') && 'jargon'.includes('on'))
```
6. _I hope this course is not full of jargon_. Check if _jargon_ is in the sentence.
```js
console.log('I hope this course is not full of jargon'.includes('jargon'))
```
7. Generate a random number between 0 and 100 inclusively.
```js
console.log(Math.floor(Math.random () * 101))
```
8. Generate a random number between 50 and 100 inclusively.
```js
console.log(Math.floor(Math.random () * 51) + 50)
```
9. Generate a random number between 0 and 255 inclusively.
```js
console.log(Math.floor(Math.random () * 256))
```
10. Access the 'JavaScript' string characters using a random number.
```js
console.log('JavaScript'[Math.floor(Math.random() * 'JavaScript'.length)])
```
11. Use console.log() and escape characters to print the following pattern.
    ```js
    1 1 1 1 1
    2 1 2 4 8
    3 1 3 9 27
    4 1 4 16 64
    5 1 5 25 125
    ```
```js
console.log('1\t1\t1\t1\t1\n2\t1\t2\t4\t8\n3\t1\t3\t9\t27')
console.log('1\t1**0\t1**1\t1**2\t1**3\n2\t2**0\t2**1\t2**2\t2**3')
```
12.  Use __substr__ to slice out the phrase __because because because__ from the following sentence:__'You cannot end a sentence with because because because is a conjunction'__
```

```

### Exercises: Level 3

1. 'Love is the best thing in this world. Some found their love and some are still looking for their love.' Count the number of word __love__ in this sentence.
2. Use __match()__ to count the number of all __because__ in the following sentence:__'You cannot end a sentence with because because because is a conjunction'__
3. Clean the following text and find the most frequent word (hint, use replace and regular expressions).

    ```js
        const sentence = '%I $am@% a %tea@cher%, &and& I lo%#ve %te@a@ching%;. The@re $is no@th@ing; &as& mo@re rewarding as educa@ting &and& @emp%o@weri@ng peo@ple. ;I found tea@ching m%o@re interesting tha@n any ot#her %jo@bs. %Do@es thi%s mo@tiv#ate yo@u to be a tea@cher!? %Th#is 30#Days&OfJavaScript &is al@so $the $resu@lt of &love& of tea&ching'
    ```

4. Calculate the total annual income of the person by extracting the numbers from the following text. 'He earns 5000 euro from salary per month, 10000 euro annual bonus, 15000 euro online courses per month.'