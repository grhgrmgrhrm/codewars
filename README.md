## Number of Decimal Digits

https://www.codewars.com/kata/number-of-decimal-digits

### en: 
Determine the total number of digits in the integer (n>=0) given as input to the function. For example, 9 is a single digit, 66 has 2 digits and 128685 has 6 digits. Be careful to avoid overflows/underflows.

### ru: 
Определите общее количество цифр в целом числе (n>=0), заданном в качестве входных данных для функции. Например, 9 - это одна цифра, 66 состоит из 2 цифр, а 128685 состоит из 6 цифр. Будьте осторожны, чтобы избежать переполнения / переполнения.

## Solution 1

```
function digits(n) {
  return n.toString().length;
}

```

## Solution 2

```
function digits(n) {
  return String(n).length
}

```

## Solution 3

```
function digits(n) {
  return `${n}`.length;
}
```

## Solution 4

```
const digits = n => n.toString().length;
```
