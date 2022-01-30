## can we divide it
https://www.codewars.com/kata/can-we-divide-it

en: Your task is to create the function isDivideBy (or is_divide_by) to check if an integer number is divisible by both integers a and b.

ru: Ваша задача состоит в том, чтобы создать функцию isDivideBy (или is_divide_by), чтобы проверить, делится ли целое число на оба целых числа a и b.

A few cases:

```
(-12, 2, -6)  ->  true
(-12, 2, -5)  ->  false

(45, 1, 6)    ->  false
(45, 5, 15)   ->  true

(4, 1, 4)     ->  true
(15, -5, 3)   ->  true
```

## Solution 1
```
function isDivideBy(number, a, b) {
  if (  number % a ===0 && number % b === 0 ) {
    return true
  } else {
    return false
  }
}
```

## Solution 2
```
const isDivideBy = (number, a, b) => number % a === 0 && number % b === 0;

```

## Solution 3
```

function isDivideBy(number, a, b) {
  return [a, b].every(i => number % i === 0)
}

```

## Solution 4
```

function isDivideBy(number, a, b) {
  return (number%a + number%b) === 0
}

```
