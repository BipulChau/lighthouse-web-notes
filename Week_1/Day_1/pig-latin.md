# Pig Latin Trasnlator
Write a program that takes any number of command line arguments, converts each to pig latin (the rules are in the next paragraph), then puts the translated words together into one sentence logged to the console.

The true pig latin rules would be a bit difficult to implement, so let's simplify them. Convert a word to pig latin by taking its first letter, moving it to the end of the word, then adding "ay" after it all.


```javascript
let details = process.argv;
let word = details.slice(2);
let pigLatin = [];

for (let i = 0; i < word.length; i++) {
  let newWord =  word[i].slice(1) + word[i][0] + "ay";
  pigLatin.push(newWord);
}

console.log(pigLatin.join(" "));
```