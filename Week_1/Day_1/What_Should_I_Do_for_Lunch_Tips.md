### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

Below is the function created in the assignment:

```javascript
const whatToDoForLunch = function (hungry, availableTime) {
  if (!hungry) {
    return console.log("Time to get back to work.");
  }
  if (availableTime < 20) {
    console.log("Pick up a snack or eat at home.");
  } else if (availableTime >= 20 && availableTime <= 30) {
    console.log("You deserve a break and should take time to cook a tasty meal.");
  } else {
    console.log("Please reconsider how much time you have.");
  }
};
```