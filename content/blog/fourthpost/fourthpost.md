---
title: Psuedocode and Comments
description: This is a post on My Blog about psuedocode and comments
date: 2024-03-02
tags: ['psuedocode', 'comments']
---
## Psuedocode
Being a computer science and ICT teacher has allowed me to encounter psuedocode with GCSE students. It has always been part of the curriculum where there is such amiguity and no particular right way of 'doing it', no industry standard and therefore when marking students' work it has been an arduous task to know whether it is 'right' or not. Completing this week's session on psuedocode has left me a little clearer on the concept of psuedocode and the use within industry but there seems to indeed be a place for it especially if you are working with the end user and non-tech personnel.


I have completed 3 different take-away tasks this week and I have documented below my attempt of them. My take-away knowledge from the session is to:
- include keywords and capitalise them, for example, PRINT, FUNCTION, etc.
- be specific in your descriptions
- do not use techy shorthand even if you know what the solution will look like - end users will not understand it and you will have to then explain further.

Essentially psuedocode's purpose is to allow you to focus on the problem away from the scenario it is contained in and is language agnostic.

We learnt also about the use and benefit of using psuedocode in interviews as if you have a clear 'plan' of what you need to implement but then either run out of time/ come into trouble trying to debug your code then the interviewer can see that you approached the task with a certain methodology and also what you intended to implement eventually.

*Take-away tasks:*
```
PSUEDOCODE AND COMMENTS TAKE AWAY TASKS (29/02/24)
Produce a pseudocode response to one or more of the following challenges. As comments.

1/FIXSTART
Create a function called fixStart. It should take a single argument, a string, and return a version where all occurrences of its first character have been replaced with ‘*’, except for the first character itself. You can assume that the string is at least one character long. For example:

fixStart('babble'): 'ba**le'
fixStart('turtle'): 'tur*le'
fixStart('and'): 'and'

START
FUNCTION accepts a single argument as a string
  TAKE first value of string
  STORE value to variable called SEARCH

  CREATE variable RESULT to store new version of argument

  FOR each value in the length of the string starting at second character and ending at last character
    IF first character == SEARCH THEN
      ADD "*"" to RESULT list
    ELSE
      ADD character to RESULT list
    END IF
  END FOR

  RETURN RESULT as output
END FUNCTION
END

2/BOOKS
Keep track of which books you read and which books you want to read!
Create a list of objects, where each object describes a book and has properties for the title (a string), author (a string), and already read (a boolean (true/false) indicating if you read it yet).
Iterate (go through) through the array of books. For each book, log the book title and book author like so: “The Hobbit by J.R.R. Tolkien”.
Modify the output based on whether the book’s been read: if so, log a string like ‘You already read “The Hobbit” by J.R.R. Tolkien’, and if not, log a string like ‘You still need to read “The Hobbit” by J.R.R. Tolkien.’

START
CREATE a list of book storing each book with title, author, isRead

FOR each book in the list
  IF already isRead === true THEN
    PRINT "You already ready read" book title "by" author
  ELSE
    PRINT "You still need to read" book title "by" author
	END IF
END FOR
END


3/RECIPE
Create an object to hold information on your favourite recipes. It should have properties for:
recipeTitle (a string)
servings (a number)
ingredients (an array of strings)
directions (a string)
List all recipes
Create a loop to list all the ingredients.


START
CREATE an object to hold specific information on favourite recipes in the following properties recipeTitle, servings, ingredients, directions.

DISPLAY each recipe in a list.
FOR each recipe in the list
  PRINT ingredients one after another.
END FOR
END
```

## Comments
Comments are important to use in your code for a number of reasons:
- when you return to code you can see what parts of your code do quickly
- you can section out parts of code when debugging
- you can include different types of comments to show for example a question about code you may have (?), a warning (!), something that is important (*).
- if other developers are reading your code then it is clearer to them what your code does by using comments.

*Different types of comments:*
Single line --> //
Multiline   --> /* */
HTML        --> !<--  -->


Comments for a function could be similar to the example below in a multiline example:

purpose of function
return no value
accepts no parameter




