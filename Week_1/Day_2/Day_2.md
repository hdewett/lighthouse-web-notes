# Day 2

## Lecture Summary

- Curriculum Overview
- Approach to lectures
- Tools
- Git / Github
- Incremental developement

We used the sum demo to demonstrate the incremental development approach. The step-by-step process that breaks down as follow:

- State the hypothesis
- Verify the hypothesis
  changes
- Rinse and repeat

For our sum problem, we broke down our problem into several steps without thinking about syntax (think pseudocode). We used consol.log efficiently to validate our assumptions and see what is really happening.

Once our solution was obtained, we did refactor our code to make it more reusable and more readable.

[sum.js demo file](https://github.com/DominicTremblay/w1d2demo-eastnov14/blob/main/sum.js)

Most important: extracting command line arguments

```javascript
const args = process.argv.slice(2);
console.log("arguments", args);
```

## Lecture Notes

- _git add ._ adds all files, same with git add
- when the files are green = files are ready to be committed, git status
- commit messages should be short but meaningful "initial commit, create sum.js"
- _git log_ = list of sommits, commit ID, author, and date
- when changing a file, git status will show that the file is red, have to do git add and then git commit again.
- _git remote -v_ will output nothing if we havent connected to a repo
- _git remote add origin SSHlinkhere_ will connect the repo you made on github
- _git branch -M main_, is used to rename the master branch to main! This literally only changes the name master to main
- _git checkout_ with the git ID, will create a new branch

## Tips

- double click a variable name, right-click, rename, change name, enter. This will change the variable names for all variables.
- for loop structure to cycle through actual elements

```javascript
let items = ["cherry", "grape", "apple"];
for (let item of items) {
  console.log(item);
  // this will print out: cherry, grape, apple
}
```

- for loop structure to cycle through index of items

```javascript
let items = ["cherry", "grape", "apple"];
for (let item in items) {
  console.log(item);
  // this will print out: 0,1,2
}
```

- spread operator: copies an array

```javascript
let items = ["cherry", "grape", "apple"];
let itemsCopy = [...items];
// this will copy items array into itemsCopy
```
