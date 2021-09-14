# Reverse a String

#### Command Line Arguments

Program that takes any number of command line arguments, all strings, and reverse them before outputting them one at a time to the console.

``` javascript
let word = process.argv;
let newWord = word.slice(2)
let reverse = []
for (let i = 0; i < newWord.length; i++){
  reverse = [];
  let wordReversed = newWord[i].split("");
  //console.log(wordReversed)
  for (let j = (wordReversed.length - 1); j >= 0; j--){
    reverse.push(wordReversed[j]);
  }    console.log (reverse.join(""))

}
```