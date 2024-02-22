---
title: This is my third post.
description: This is a post on My Blog about win-win survival strategies.
date: 2018-08-24
tags:
  - second tag
  - posts with two tags
---
Leverage agile frameworks to provide a robust synopsis for high level overviews. Iterative approaches to corporate strategy foster collaborative thinking to further the overall value proposition. Organically grow the holistic world view of disruptive innovation via workplace diversity and empowerment.

## Code

### Styled (with Syntax)

Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved from generation X is on the runway heading towards a streamlined cloud solution. User generated content in real-time will have multiple touchpoints for offshoring.

```js
//Task 1
//program to work out a pecentage of a number

function percentageCalculator(a, b) {
  return (a / 100) * b;
}

//can use the code below to set a number or uncomment the script in the html to create an alert prompt to gather the input to use in the calculator.
const percentage = 30;
const number = 135;

//creates variable result with the value returned from function.
const result = percentageCalculator(percentage, number);

//prints out the result in a sentence
console.log("The result of", percentage, "% of", number, "is", result);

//Task 2
//soft drink machine
//function which takes arguments for size and flavour
function drinkOrder(size, buttonLabel) {
  let drink = ""; //empty variable for name of choice.

  switch (buttonLabel) {
    case "Cola":
      drink = "Coca-cola";
      break;
    case "lemon":
      drink = "Lemonade";
      break;
    case "orange":
      drink = "Orangeade";
      break;
    default:
      drink = "Not available";
  }
  //output the message with the size and then the correct drink label.
  console.log("You have ordered a", size, drink);
}
//passing different options into function to check it works
drinkOrder("small", "Cola");
drinkOrder("medium", "orange");
drinkOrder("large", "lemon");
drinkOrder("large", "malibu");

//Task 3

//function passes 2 numbers and operator.
function calculator(number1, number2, operator) {
  let value = "";
  //switch to check the operator and return the value of the 'sum' dependant on the operator.
  switch (operator) {
    case "+":
      value = number1 + number2;
      break;
    case "-":
      value = number1 - number2;
      break;
    case "*":
      value = number1 * number2;
      break;
    case "/":
      value = number1 / number2;
      break;
    case "%":
      value = number1 % number2;
      break;
    //can also return the values instead.
  }
  //outputs the logic and the value.
  console.log(number1, operator, number2, "=", value);
}

//options to pass throught the function to see if they all work.
calculator(2, 4, "+");
calculator(2, 4, "-");
calculator(2, 4, "*");
calculator(2, 4, "/");
calculator(2, 4, "%");

```

### Unstyled

Bring to the table win-win survival strategies to ensure proactive domination. At the end of the day, going forward, a new normal that has evolved from generation X is on the runway heading towards a streamlined cloud solution. User generated content in real-time will have multiple touchpoints for offshoring.

```
// this is a command
function myCommand() {
	let counter = 0;
	counter++;
}

// Test with a line break above this line.
console.log('Test');
```

## Section Header

Capitalize on low hanging fruit to identify a ballpark value added activity to beta test. Override the digital divide with additional clickthroughs from DevOps. Nanotechnology immersion along the information highway will close the loop on focusing solely on the bottom line.
