## can we divide it
https://www.codewars.com/kata/can-we-divide-it


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
