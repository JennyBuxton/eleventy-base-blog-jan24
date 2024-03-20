---
title: Loops, Arrays and Objects in Javascript
date: 2024-03-20
description: This is a post on My Blog about using loops, arrays and objects in Javascript/
tags: ['eleventy', 'javascript', 'loops', 'arrays', 'objects']
---
# Loops, Arrays and Objects

This is where it started to get pretty hard.
I have always sturggled with getting my head around functions especially which I have been told is common. This has been no different with Javascript.

I have managed to create solutions to the the tasks but this has taken me a while and they are not all perfect but I realise that practice makes perfect.

## Loops

```
for (let i = 1; i < 13; i++) {
 // console.log(i)
  console.log(`this is i = ${i}`)
}
```
Simple for loop which prints out this is i and the number from 1-12 next to each one.

## Arrays

```
console.log([]);

console.log([1, 2, 3, 4]);

console.log([1, "true", 3, [1, 2, 3]]);

//Different ways to add and remove
const arr = [1, 2, 3, 4];
arr.push(3);
arr.pop();
arr.shift();
arr.unshift(0);

console.log(arr);
```
Looking at different things you can do with the data in an array. You can have different data types in the same array.

## Objects

```
const obj1 = {
  fName: "Foo",
  sName: "Bar",
  dob: new Date()
};
//print out the object
console.log(obj1);

//print out the fName in the object
console.log(obj1.fName);

//add key - age to the object and assign value 34
//Then print out the object
obj1.age = 34;
console.log(obj1);

//add key - email to the object and assign value "ada@ada.com"
//Then print out the object
obj1.email = "ada@ada.com";
console.log(obj1);
```
Here I created a small object and added some key:value pairs to it.
When handling objects you use dot notation.

Below are the takeaway tasks that were set to practice our skills this week in all 3 new skills learnt.

```
//Task 1

//Write a loop that outputs the 7 times table,

//from 7 x 1 = 7 to 7 x 12 = 84

const number = 7

for (let i = 1;i<13; i++){
  let sum = number*i;
  console.log(`${number} x ${i} = ${sum}`)
}


//Task 2

//Create an array of your favourite foods.

//Print some of them to the screen

const faveFoods = ["sausage", "pizza", "cheese", "cucumber", "ice-cream"];

console.log(faveFoods[1]);
console.log(faveFoods[3]);
console.log(faveFoods[0]);


//Task 3
//Use a for loop to print a list of all your favourite foods
for (var i = 0; i < faveFoods.length; i++) {
    console.log(faveFoods[i]);
}



//Task 4

//Create an object to hold information on your favourite recipe. Then display the properties on screen.


const recipe = {};

recipe.title = "Chilli Con Carne";
recipe.servings = 4;
recipe.ingredients = [
  "beef mince",
  "dark chocolate",
  "chopped tomatoes",
  "hot chilli powder",
  "paprika",
  "cumin",
  "oregano",
  "kidney beans",
  "tomato paste",
  "salt",
  "pepper",
  "oil",
  "red pepper",
  "onion",
  "garlic",
  "beef stock cube"
];
recipe.directions = [
  " STEP 1: Chop 1 large onion into small dice",
  "STEP 2: Cut 1 red pepper in half lengthways, remove stalk and wash the seeds away, then chop. Peel and finely chop 2 garlic cloves",
  "STEP 3: Start cooking. Put your pan on the hob over a medium heat. Add 1 tbsp oil and leave it for 1-2 minutes until hot (a little longer for an electric hob).",
  "STEP 4: Add the onion and cook, stirring fairly frequently, for about 5 minutes, or until the onion is soft, squidgy and slightly translucent.",
  "STEP 5: Tip in the garlic, red pepper, 1 heaped tsp hot chilli powder or 1 level tbsp mild chilli powder, 1 tsp paprika and 1 tsp ground cumin.",
  "STEP 6: Give it a good stir, then leave it to cook for another 5 minutes, stirring occasionally.",
  "STEP 7: Brown 500g lean minced beef. Turn the heat up a bit, add the meat to the pan and break it up with your spoon or spatula. The mix should sizzle a bit when you add the mince.",
  "STEP 8: Keep stirring and prodding for at least 5 minutes, until all the mince is in uniform, mince-sized lumps and there are no more pink bits. Make sure you keep the heat hot enough for the meat to fry and become brown, rather than just stew.",
  "STEP 9: Make the sauce. Crumble 1 beef stock cube into 300ml hot water. Pour this into the pan with the mince mixture.",
  "STEP 10: Add a 400g can of chopped tomatoes. Tip in ½ tsp dried marjoram, 1 tsp sugar and add a good shake of salt and pepper. Squirt in about 2 tbsp tomato purée and stir the sauce well.",
  "STEP 11: Simmer it gently. Bring the whole thing to the boil, give it a good stir and put a lid on the pan. Turn down the heat until it is gently bubbling and leave it for 20 minutes.",
  "STEP 12:Check on the pan occasionally to stir it and make sure the sauce doesn’t catch on the bottom of the pan or isn’t drying out. If it is, add a couple of tablespoons of water and make sure that the heat really is low enough. After simmering gently, the saucy mince mixture should look thick, moist and juicy.",
  "STEP 13: Drain and rinse a 410g can of red kidney beans in a sieve and stir them into the chilli pot. Bring to the boil again, and gently bubble without the lid for another 10 minutes, adding a little more water if it looks too dry.",
  "STEP 14: Taste a bit of the chilli and season. It will probably take a lot more seasoning than you think.",
  "STEP 15: Now replace the lid, turn off the heat and leave your chilli to stand for 10 minutes before serving. This is really important as it allows the flavours to mingle.",
  "STEP 16: Serve with soured cream and plain boiled long grain rice."
];

console.log(recipe.title);
console.log("Serves", recipe.servings);
console.log("Serves", recipe.ingredients);
console.log("Serves", recipe.directions);


//Bonus Points: Create a loop to list all the ingredients and directions.

let recipeArr = Object.entries(recipe);

console.log(recipeArr);

//Task 5

//Add a function called letsCook

//Have it say: "I'm hungry! Let's cook..." with the name of your recipe title.

//Call your new method.

function letsCook(title) {
 console.log(`I'm hungry! Let's cook...${recipe.title}`)
};

letsCook('anything');
```



