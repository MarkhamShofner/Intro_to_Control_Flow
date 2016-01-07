# Introduction to Control Flow

## Learning Objectives
- Describe what control flow is
- Understand the various ways control flow can be used
- Implement self-built examples of control flow (primarily conditionals)
  - Time permitting, intro to loops

## Basics of Control Flow
#### Introduce Topic & explain skill – I DO (5 min)
<!-- draw on whiteboard, use visual aids/discussion -->
In computer science, control flow (or alternatively, flow of control) is the order in which individual statements, instructions or function calls of an imperative program are executed or evaluated.

Primary
- conditionals (if-then, if-then-else)
  - the focus of today's lesson
- for loops
- while loops

Additional
- switch statements
- do-while statements

##### Turn and Talk
  > Examples of conditionals you've worked through outside of programming

##### Group Discussion
  > Share interesting points

##### Some other examples
- Decision trees
- Process mapping
- Stories

Why we need to be precise in our language? Computers cannot read between the lines.

  >A wife asks her husband, a computer programmer;
  "Could you please go to the store for me and buy one carton of milk, and if they have eggs, get 6!"
  A short time later the husband comes back with 6 cartons of milk.
  The wife asks him, "Why the hell did you buy 6 cartons of milk?"
  He replied, "They had eggs."

Coding humor.

#####Fist to five check-in.

***

#### Practice Skill together – WE DO (5 min)
Write a function that accepts a plane ticket cost, and logs "Too Expensive", "Seems Reasonable", and "Buy Buy Buy!" at $500, $250, $100 ranges respectively.
If the cost is above $500 log "I'm not made of money!".

```javascript
function ticketCost (x) {
    if (/*condition to be met*/) {
      //code to execute
    }
}

```

Take a few minutes to build out the above structure before moving on to the answer below.

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
- Shout out some others!

##### Additional Control Flow
Time permitting, set up intro exposure to loops.

#### Review Questions
1. Why use control flow in the first place?
2. What are some good practices to implement while writing control flow?
3. What is the most basic form of control flow?

##### Further Research
- FizzBuzz
  - https://www.codecademy.com/courses/fizzbuzz/0/1
- https://en.wikipedia.org/wiki/Decision_tree
- Text-based adventure games
