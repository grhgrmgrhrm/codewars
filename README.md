## Capitalization and Mutability

https://www.codewars.com/kata/capitalization-and-mutability

### en: 
Your coworker was supposed to write a simple helper function to capitalize a string (that contains a single word) before they went on vacation.

Unfortunately, they have now left and the code they gave you doesn't work. Fix the helper function they wrote so that it works as intended (i.e. make the first character in the string "word" upper case).

Don't worry about numbers, special characters, or non-string types being passed to the function. The string lengths will be from 1 character up to 10 characters, but will never be empty.


### ru: 
Предполагалось, что ваш коллега напишет простую вспомогательную функцию для заглавной строки (содержащей одно слово), прежде чем отправиться в отпуск.

К сожалению, сейчас они ушли, и код, который они вам дали, не работает. Исправьте вспомогательную функцию, которую они написали, чтобы она работала так, как задумано (т.Е. сделайте первый символ в строке "слово" прописным).

Не беспокойтесь о том, что в функцию передаются числа, специальные символы или нестроковые типы. Длина строки будет составлять от 1 символа до 10 символов, но никогда не будет пустой.


## Solution 1
```
function capitalizeWord(word) {
  return word[0].toUpperCase() + word.slice(1);
}

```

## Solution 2
```
const capitalizeWord = (word) => word.replace(word.charAt(0), word.charAt(0).toUpperCase());

```

## Solution 3
```
const capitalizeWord = word => word[0].toUpperCase()+word.slice(1);

```

## Solution 4
```
function capitalizeWord(word) {
  return word[0].toUpperCase() + word.slice(1).toLowerCase();
}

```
