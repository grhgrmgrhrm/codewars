## Convert a String to a Number!

https://www.codewars.com/kata/convert-a-string-to-a-number

### en: 
We need a function that can transform a string into a number. What ways of achieving this do you know?

Note: Don't worry, all inputs will be strings, and every string is a perfectly valid representation of an integral number.


### ru: 
Нам нужна функция, которая может преобразовать строку в число. Какие способы достижения этой цели вы знаете?

Примечание: Не волнуйтесь, все входные данные будут строками, и каждая строка является абсолютно корректным представлением целого числа.

### Examples

```
"1234" --> 1234
"605"  --> 605
"1405" --> 1405
"-7" --> -7
```


## Solution 1
```
var stringToNumber = function(str){
  return +str;
}

```

## Solution 2
```
var stringToNumber = function(str){
  return parseInt(str);
}

```

## Solution 3
```
var stringToNumber = function(str){
  return Number(str);
}

```

## Solution 4
```
var stringToNumber = Number;

```
