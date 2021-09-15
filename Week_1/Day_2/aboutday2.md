# Day 2
Today we had our first lecture. We learned about Dev Workflow. Today's notes from the lecture are here below:

* 7 Programming test - Just problem solving
* week 2, 4 & 9 - Tech Interviews
* Quizzes - Till 5th week
* To raise your hand - use Option + Y key in zoom
* Useful add-ons in VS code - eslint, bracket matching and prettier. Bracket Pair Colorizer 2

### Git commands:
* git add _A / git add . /git add * - all does the same function of adding all files to the stage

* ls -al, git remote -v, git remote -rm origin, git branch, git push -u origin master, git branch -M main

### Edge Case:
What to do when arguments are not as per specified

### parseInt() 
It will change the number into whole number.
parseInt(5.5) - 5
parseInt("5.5") - 5
parseInt("5Hello") - 5

* Usually rerturn is placed inside a function
* process.exit() -  to stop the process/code from running
* Number.isInteger(9) - true - to check if the number is an integer.
* For arrays and objects it is perfectly ok to use const

## Array.filter((element)=>element != xyz):
This filter function of array returns a new filter. Eg is as follows:
let shoppingList = ["Apple", "Oranges", "Apple", "Tomato", "Fish"]
let newShoppingList = shoppingList.filter((list)=> list !== "Apple")

The above code will output:  
newShoppingList =["Oranges", "Tomato", "Fish"]

Following is the function created using filter() which will create a subset of given arrays removing some elements:

```javascript
const without = function(source, itemToRemove) {
  for (let i = 0; i < itemToRemove.length; i++) {
    let newArr = source.filter((item)=> item !== itemToRemove[i]);
    source = newArr;
  } return source;
};
```



