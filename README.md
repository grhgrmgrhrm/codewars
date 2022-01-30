## Convert a Number to a String!

https://www.codewars.com/kata/convert-a-number-to-a-string

### en: 
We need a function that can transform a number into a string.

What ways of achieving this do you know?


### ru: 
Нам нужна функция, которая может преобразовать число в строку.

Какие способы достижения этой цели вы знаете?

Examples

```
123 --> "123"
999 --> "999"
```


## Solution 1
```
function numberToString(num) {
  return num.toString();
}
```

## Solution 2
```
function numberToString(num) {
  // Return a string of the number here!
  return String(num);
}

```

## Solution 3
```
function numberToString(num) {
  return ''+num;
}

```

## Solution 4
```
const numberToString = num => num.toString();

```
