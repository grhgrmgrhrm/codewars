## Fake binary

https://www.codewars.com/kata/fake-binary/javascript

### en: 
Given a string of digits, you should replace any digit below 5 with '0' and any digit 5 and above with '1'. Return the resulting string.

Note: input will never be an empty string


### ru: 
Учитывая строку цифр, вы должны заменить любую цифру ниже 5 на "0", а любую цифру 5 и выше - на "1". Верните результирующую строку.

Примечание: ввод никогда не будет пустой строкой


## Solution 1

```
function fakeBin(x){
  let newStr = "";
  for(let i=0; i < x.length; i++){
    if (+x[i] >= 5) {
      newStr += "1";
    } else {
      newStr += "0";
    }
  }
  return newStr;
}

```

## Solution 2

```
function fakeBin(x) {
    return x.split('').map(n => n < 5 ? 0 : 1).join('');
}

```

## Solution 3

```

function fakeBin(x) {
  return x.replace(/\d/g, d => d < 5 ? 0 : 1);
}

```

## Solution 4

```
function fakeBin(x){
  let result = '';
  for(let i = 0; i < x.length; i++){
    x[i] < 5 ? result += 0 : result += 1;
  }
  return result;
}

```
