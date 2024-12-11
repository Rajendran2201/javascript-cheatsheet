# Getting started with JavaScript

>**Where did JavaScript originate from?**
- Javascript didn't come up through the ivy leagues with careful consideration. Instead, It came out of necessity into the internet. So, It has a lot of good part and some not so good parts as well.

All these days, we have been writing code or building web pages with HTML and CSS. Though they are fascinating, they are static and boring. So here we are to learn JavaScript, a way of introducing behavior and dynamicity to our we pages. 

### Getting started with JavaScript

```html
<!DOCTYPE html>

<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Document</title>

<script>

console.log("Hey buddy, kudos to you for learning js!")

</script>

</head>

<body>

</body>

</html>
```


![](https://i.imgur.com/S6Bi0EQ.png)

> So, this is how we can get Javascript into the webpage. 

There is another way to write your javascript code in a separate file and link it to the HTML. we'll look into it as well.

**How to link external js file with HTML?**

This is possible by inserting `<script defer src="js-file.js"></script>`.

> **Why to use `defer` ?**  Usually when we add script file in head, the compiler parses the HTML file sequentially from top to bottom. But when it reaches the script file, it redirects to it. Thus not reading the code below the script file immediately. To avoid it, we use `defer`.

![](https://i.imgur.com/IYNMhY2.png)


![](https://i.imgur.com/iBwEbjF.png)

### Then, where did JavaScript actually originate from?

- The roots of javascript comes from Netscape, the first browser company. They created a scripting language that would allow anyone to add scripts to their pages and named it as Livescript in 1995.
- During the same time, Sun Microsystems introduced Java and it became incredibly popular. So to capitalize on that success, Livescript was renamed as Javascript.
