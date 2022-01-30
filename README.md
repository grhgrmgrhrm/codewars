## Century From Year

https://www.codewars.com/kata/century-from-year

### en: 
Introduction

The first century spans from the year 1 up to and including the year 100, the second century - from the year 101 up to and including the year 200, etc.
Task

Given a year, return the century it is in.


### ru: 
Вступление

Первое столетие охватывает период с 1 года до 100 года включительно, второе столетие - с 101 года до 200 года включительно и т.д.
Задача

Учитывая год, верните столетие, в котором оно находится.

Examples

```
1705 --> 18
1900 --> 19
1601 --> 17
2000 --> 20
```


## Solution 1
```
const century = year => Math.ceil(year/100)

```

## Solution 2
```
function century(year) {
  return Math.ceil(year/100); //using ceiling method to round up to nearest century (100)
}

```

## Solution 3
```
function century(year) {
  return (year + 99) / 100 | 0;
}

```

## Solution 4
```
const century = year => year % 100 === 0 ? parseInt(year / 100) : parseInt(year / 100) + 1;

```
