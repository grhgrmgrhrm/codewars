## Largest Square Inside A Circle

https://www.codewars.com/kata/largest-square-inside-a-circle

### en: 
Determine the area of the largest square that can fit inside a circle with radius r.


### ru: 
Определите площадь наибольшего квадрата, который может поместиться внутри круга радиусом r.


## Solution 1

```
function areaLargestSquare(r) {
  return r*r*2; 
}

```

## Solution 2

```
var areaLargestSquare = r => r**2 + r**2

```

## Solution 3

```
const areaLargestSquare = (radius) => Math.pow(radius, 2) * 2 

```

## Solution 4

```
areaLargestSquare=(r)=>2*r**2

```
