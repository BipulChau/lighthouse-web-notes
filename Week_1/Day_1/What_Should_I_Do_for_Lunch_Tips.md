### Tips

Try experimenting with the compasriosn operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant. 

Work on your code iteratively - that meand in small pieces. 

To help your figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript
const whatToDoForLunch = function(hungry, availableTime) {
  if (hungry) {
    if (availableTime > 30) {
      console.log(
        "You're in a bootcamp and should reconsider how much time you actually have to spare"
      );
    } else if (availableTime >= 20) {
      console.log("Try a place nearby");
    } else {
      console.log("Pick something up and eat in the lab");
    }
  } else {
    console.log("Get back to work");
  }
};
```