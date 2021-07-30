## Valid Braces
https://www.codewars.com/kata/5277c8a221e209d3f6000b56


## Solution 1
```
function validBraces(braces){
  var matches = { '(':')', '{':'}', '[':']' };
  var stack = [];
  var currentChar;

  for (var i=0; i<braces.length; i++) {
    currentChar = braces[i];

    if (matches[currentChar]) { // opening braces
      stack.push(currentChar);
    } else { // closing braces
      if (currentChar !== matches[stack.pop()]) {
        return false;
      }
    }
  }

  return stack.length === 0; // any unclosed braces left?
}
```

## Solution 2
```
function validBraces(braces){
  var queue = [];

  for(var brace of braces) {
    if(brace === '(' || brace === '{' || brace === '[') {
      queue.push(brace);
    } else {
      var last = queue.pop();
      if(last === '(' && brace === ')') {
        continue;
      } else if (last === '[' && brace === ']') {
        continue;
      } else if (last === '{' && brace === '}') {
        continue;
      } else {
        return false;
      }
    }
  }
  
  return queue.length === 0;
}
```

## Solution 3
```
function validBraces(braces){
  var matches = { '(':')', '{':'}', '[':']' };
  var queue = [];

  for(var brace of braces) {
    if (matches[brace]) {
      queue.push(brace);
    } else {
      if (brace !== matches[queue.pop()]) {
        return false;
      }
    }
  }

  return queue.length === 0;
}
```

## Solution 4
```
function validBraces(braces){
  while(braces.indexOf("{}") != -1 || braces.indexOf("()") != -1 || braces.indexOf("[]") != -1){
    braces = braces.replace("{}", "").replace("()", "").replace("[]", "");
  }
```
  
  return braces.length == 0;
}
