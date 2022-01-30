## Convert to Binary

https://www.codewars.com/kata/convert-to-binary

### en: 
We need a function that can transform a string into a number. What ways of achieving this do you know?

Note: Don't worry, all inputs will be strings, and every string is a perfectly valid representation of an integral number.


### ru: 
Учитывая неотрицательное целое число n, напишите функцию to_binary/To Binary, которая возвращает это число в двоичном формате.

### Examples

```
toBinary(1)  /* should return 1 */
toBinary(5)  /* should return 101 */
toBinary(11) /* should return 1011 */

```


## Solution 1

```
let toBinary = n => +n.toString(2)

```

## Solution 2

```
toBinary = (n) => parseInt(n.toString(2));

```

## Solution 3

```
function toBinary(n){
  return +n.toString(2);
}

```

## Solution 4

```
const toBinary = n => Number(n.toString(2)) ;

```
