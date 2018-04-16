# Whale-Talk

Like Finding Nemo, just a little bit less cute.

## Loops, Loops, all about Loops

### What I learned:

#### For Loops:

* **for** loops let us loop a block of code, a know number of times.

Example:

```
let myGitHubRepos = ['DogYearsCalc', 'Magic8Ball', 'RaceRegistrationApp'];

for (let i=0;i<myGitHubRepos.length;i++){
 console.log(myGitHubRepos[i]);
}
```

* **"let i=0;"** the first part of the **for** loop is the _start condition_, and declares an _iterator variable_ to start from.
* **i<gitHubRepos.length;** the second part of the loop is the **stop condition**, and the loop will continue to execute forever, while the stop condition is still true.
* **i++** the third part of the loop is the _iterator_
* **{console.log(gitHubRepos[i]);}** the last part of the loop is the _code block_ and will execute until the program reaches the stop condition.

* How might we make a **for loop** run backwards?
  * We set the start condition equal to the length of the array, minus 1.

#### Nested For Loops

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

#### While Loops:

* **while** loops let us loop a block of code, while a certain condition is true.
