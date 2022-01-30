## Even or Odd

https://www.codewars.com/kata/even-or-odd

### en: 
Create a function that takes an integer as an argument and returns "Even" for even numbers or "Odd" for odd numbers.


### ru: 
Создайте функцию, которая принимает целое число в качестве аргумента и возвращает "Четное" для четных чисел или "Нечетное" для нечетных чисел.




## Solution 1

```
function even_or_odd(number) {
  if (number%2 == 0) {
    return "Even";
  } else {
    return "Odd";
  }
}

```

## Solution 2

```
function even_or_odd(number) {
  return number % 2 ? "Odd" : "Even"
}

```

## Solution 3

```
function even_or_odd(number) {
   return number % 2 === 0 ? 'Even' : 'Odd';
}
```

## Solution 4

```
const even_or_odd = n => (n % 2) ? 'Odd' : 'Even';
```
