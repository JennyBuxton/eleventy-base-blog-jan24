---
title: Coder's Guild Web Development Course.
description: This is a post on My Blog about SSG - Static Sites and starting out.
date: 2024-01-30
	tags: ['eleventy', 'starting out']

---
## Coder's Guild Web Development Course

I am learning the skills to become a web developer with Coder's Guild.
With an already solid knowledge of html and some css through teaching at secondary school I am building on these skills and my interest in web design.

In this task I have learnt how to set up a static site and why we might use them, basically if you need a site which does not change regularly you would use a static site.

We have learnt about Eleventy and Netlify (sites are deployed to Netlify.)
Netlify is the published website - I believe Eleventy is the server.

All of this is pretty confusing at the moment but I am sure once I use it a few times then I will understand more which each software is used for exactly and how they all work together.

## HTML and CSS


This is an example of my first knowedge of html and CSS - very basic:

```diff-js
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Jen's Favourite Films</title>
  <link rel="stylesheet" href="style.css">
</head>

<body>
  <header>
    <h1 id="title" name="title"> Jenny's Favourite Films </h1>
  </header>
  <article>
    <p id="paragraph" name="paragraph"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque sit amet ex sagittis, egestas velit non, posuere erat. Proin lacinia euismod enim, ut consectetur ipsum molestie eget. </p>
  </article>

  <h2 id="films" name="films"> My top 3 films </h2>
  <ol>
    <li> <a href="https://www.imdb.com/title/tt1649419/" target="_blank">The Impossible</a></li>
    <li> <a href="https://www.imdb.com/title/tt0094721/?ref_=nv_sr_srsg_0_tt_7_nm_1_q_beetle%2520jui" target="_blank">Beetle Juice </a></li>
    <li> <a href="https://www.imdb.com/title/tt0098319/?ref_=nv_sr_srsg_0_tt_2_nm_6_q_shirley%2520val" target="_blank">Shirley Valentine</a></li>
  </ol>

</body>

</html>
```

And this is the CSS file:
```
h1 {
  font-family: arial;
  color: blue;
  text-align: center;
}

header {
  postition: absolute;

  margin: 50px;
  padding: 20px;
  background-color: lightblue;
  font-size: 20px;
  color: darkblue;
  box-shadow: 10px 5px 5px blue;
  border-radius: 25px;
}

#paragraph {
  text-align: center;
  background-color: lightblue;
  margin: 20px;
  padding: 20px;
  font-family: arial;
}
```
