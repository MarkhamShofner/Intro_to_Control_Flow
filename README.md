# Introduction to Control Flow

> Assuming the class has covered the basics of JavaScript - including variables, functions, and booleans.

## Learning Objectives
- Describe what control flow is
- Understand the various ways control flow can be used
- Implement self-built examples of control flow (primarily conditionals)

## Basics of Control Flow
#### Introduce Topic & explain skill – I DO (4 min)
<!-- draw on whiteboard, use visual aids/discussion -->
In computer science, control flow is the order in which individual statements, instructions, or functions are executed or evaluated.

#####Primary
- conditionals (if-then, if-then-else)
  - the focus of today's lesson
- for loops
- while loops

#####Additional
- switch statements
- do-while statements

##### Group Discussion
  > Share examples of conditionals you've worked through outside of programming

##### Some other examples
- Decision trees
- Process mapping

Why do we need to be precise in our language? We must be precise because computers cannot read between the lines.

  >A wife asks her husband, a computer programmer;
  "Could you please go to the store for me and buy one carton of milk, and if they have eggs, get 6!"
  A short time later the husband comes back with 6 cartons of milk.
  The wife asks him, "Why the hell did you buy 6 cartons of milk?"
  He replied, "They had eggs."

Coding humor.

***

#### Practice Skill together – WE DO (4 min)
Let's write a function that accepts a plane ticket cost, and logs:
- "Buy Buy Buy!" below $100
- "Seems Reasonable" between $100 and $200
- "Too Expensive" above $500
- "I'm not made of money!" if none of the above

```javascript
function ticketCost (x) {

    if (/*condition to be met*/) {
      /*code to execute*/
    } else if (/*secondary condition*/) {
      /*code*/
    } else if (/*tertiary condition*/) {
      /*code*/
    } else /*if no condition is met*/ {
      /*code*/
    }
}

```
Let's take a few minutes to build out a draft structure before moving on to the answer below.

- What happens if multiple conditions in the same statement are met?
  - Note that if any earlier loop is met, then the code will jump to the end of the conditional, only executing the first matching condition.
- How else can the order of conditionals be made?

```javascript
function ticketCost (x) {
    if (x < 100) {
        console.log("Buy Buy Buy!");
    } else if (x < 200) {
        console.log("Seems reasonable");
    } else if (x < 500) {
        console.log("Too expensive");
    } else {
        console.log("I'm not made of money!");
    }
}

ticketCost (50);
ticketCost (150);
ticketCost (250);
ticketCost (550);
```

##### Potential others examples of conditionals
- Height for theme park rides
- Age for entrance to clubs

##### Fist to five check-in.

##### Additional Control Flow - YOU DO (4 min)
Open up http://labs.codecademy.com/#:workspace in your browser of choice.

Reverse the order of the above ticket cost function. Instead of checking first if something is cheap enough, start from the top ceiling condition and work your way down.

#### Review Questions and Wrap-Up (2 min)
1. Why use control flow in the first place?
2. What are some good practices to implement while writing control flow?
3. What is a basic form of control flow?
4. What are some additional forms of control flow?

***

##### Bonus - Work through fizzbuzz using loops and conditionals
Model the following problem - loop from 1 through 15.
- If the number is divisible by three, log fizz
- If divisible by five, log buzz
- If divisible by both three and five, log fizzbuzz
- If none of the above conditions are met, log the number

##### Further Research
- https://www.codecademy.com/courses/fizzbuzz/0/1
- https://en.wikipedia.org/wiki/Decision_tree
- Text-based adventure games
