SURVAY SAYS!  
=============
![](https://media.giphy.com/media/ygKSRlIvaKb04/giphy.gif)  

GOAL  
-------------
The information in the database file attached here has results from a survey Jeff took of some of his friends. He's going to use that information to learn some things about the friends who answered the survey. For example:

* What percent of his friends are programmers?
* Do they like similar or dissimilar music?
* How many of them live in each state?

**One warning**: these are real people, and real people don't always provide the easiest data to work with. Get ready for typos, unexpected blanks, and outright silliness (Max, for example, isn't 100 years old).

In the `script.js` file, Jeff has written some questions he has. Use your knowledge of lists and objects to get at the information asked for in each of the 9 challenges.

TIPS AND TRICKS
-------------
Try to get a feel for the shape of the data by adding the three print statements below to the script.js file:
import database

```javascript
// All the survey responses are stored in a list called "people".
console.log(people)
console.log("THE FIRST PERSON IS:" + people[0])
// 2. Print out the name of the first person who responded to the survey
```

Then run the code and open the console:

You'll notice that the real trouble is that it's providing WAY more than that person's name. It's providing their ***ENTIRE*** object.

That means the answer to challenge 2 will look something like this:

```javascript
// 2. Print out the name of the first person who responded to the survey
console.log(people[0]["Name"])
// Using dot notation
console.log(people[0].Name)
```