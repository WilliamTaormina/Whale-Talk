# Whale-Talk: Loops, Loops, all about Loops

Whales can only speak in vowels, and they talk really loud. (Like in APP CAPS). What would a whale sound like if it was trying to read you the Odyssey, By Homer Book 1, paragraphs 1 and 2?

Find out! (Or input your own passage!)

EEEEOUUOOEEAAAA !!!

## What I learned:

### For Loops:

* **for** loops let us loop a block of code, a know number of times.

Example:

```
let myGitHubRepos = ['DogYearsCalc', 'Magic8Ball', 'RaceRegistrationApp'];

for (let i=0;i<myGitHubRepos.length;i++){
 console.log(myGitHubRepos[i]);
}
```

* **"let i=0;"**
  * the first part of the **for** loop is the _start condition_, and declares an _iterator variable_ to start from.
* **i<gitHubRepos.length;**
  * the second part of the loop is the **stop condition**, and the loop will continue to execute forever, while the stop condition is still true.
* **i++**
  * the third part of the loop is the _iterator_
* **{console.log(gitHubRepos[i]);}**

  * the last part of the loop is the _code block_ and will execute until the program reaches the stop condition.

* How might we make a **for loop** run backwards?
  * We set the start condition equal to the length of the array, minus 1.

### Nested For Loops

* Nested for loops are useful when comparing the contents of two arrays. With nested **for loops**, every time the outer for loop runs once, the inner for loop runs completely.
* Building off the example above, let's pretend that you and I want to compare all the GitHub repos we each have:

Example:

```
let myGitHubRepos = ['DogYearsCalc', 'Magic8Ball', 'RaceRegistrationApp'];
let yourGitHubRepos = ['Basketball App', 'Cat App', 'Magic8Ball']

for (let i=0;i<myGitHubRepos.length;i++){
 for (let j = 0; j<yourGitHubRepos.length; j++){
  if (myGitHubRepos[i] === yourGitHubRepos[j]){
   console.log('You both have the ' + myGitHubRepos[i] + 'repo in your account. Maybe you should chat about building a new feature!');
  }
 }
}
```

### While Loops:

* **while loops** let us loop a block of code, while a certain condition is true.
* **While Loops** work better when the number of loop iterations is randomized or variable.
* the Syntax for a **While Loop** is shown below:

```
while(condition-is-true){
 do this operation;
}
```

Here is an example while loop:

```
let cards = ['Diamond', 'Spade', 'Heart', 'Club'];

let currentCard = 'Heart';

while (currentCard != 'Spade'){
 console.log(currentCard)
  currentCard = cards[Math.floor(Math.random()*4)];
}

console.log('It looks like the program found a Spade!')
```

### BEWARE: infinite looooooooooooooooooooooops:

* an **infiinte loop** occures when a loop begins, and does not have a stop condition in place, or met. Therefore, the loop continues on forever, and will crash your machine.
* infine loops in **for loops** are less common because the start, stop, and iterating conditions are explicitly set.
* Infinite loops are more common in while loops, because if the conditional statement is set to and equals 'true', and does not have a break, the loop with go on forever.
