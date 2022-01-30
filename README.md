## Perimeter sequence

https://www.codewars.com/kata/perimeter-sequence

### en: 
The first three stages of a sequence are shown.

![images](https://user-images.githubusercontent.com/30986517/151703534-45b7233b-6112-466e-8da4-23819465caba.png)

The blocksize is a by a and a ≥ 1.

What is the perimeter of the nth shape in the sequence (n ≥ 1) ?
### ru: 

Показаны первые три этапа последовательности.

![images](https://user-images.githubusercontent.com/30986517/151703534-45b7233b-6112-466e-8da4-23819465caba.png)

Размер блока равен a на a и a ≥ 1.

Каков периметр n-й фигуры в последовательности (n ≥ 1)?

## Solution 1

```

function perimeterSequence(a,n) {
  return 4*a*n
}

```

## Solution 2

```

perimeterSequence = (a, n)  => a * n * 4;

```

## Solution 3

```

perimeterSequence = (a, n)  => a * n * 4;

```

## Solution 4

```

function perimeterSequence(a,n) {
  let sum = 0;
  for(let i = 0 ; i < n; i++) {
    sum += 4 * a;
  }
  return sum;
}

```
