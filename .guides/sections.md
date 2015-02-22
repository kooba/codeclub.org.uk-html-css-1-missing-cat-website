---
title: The Mission
files: []
layout: 2-panels-tree

---
Felix the cat has gone missing. His owner made a poster to hang up in the neighborhood, but you realise making a website means many more people can see it.

![](.guides/img/missingcat.png)

---
title: Step 1
files:
  - action: open
    path: "#cmd: bash .guides/restore.sh missing_cat,index.html"
    panel: 0
layout: ""

---
Set up your document like you learnt in the previous session

```html
<!DOCTYPE html>
<html>
    <head>
    </head>
    <body>
    </body>
</html>
```

Make a title and header. Remember the title goes in the head and the header goes in the `body`. Try using **“Felix the cat is missing”** as a title, and **Missing** as the `h1`. Right beneath the `<h1>` we can make a `<h2>` saying **“Felix the cat”**.

```html
<!DOCTYPE html>
<html>
    <head>
        <title> Felix the cat is missing </title>
    </head>
    <body>
        <h1>Missing</h1>
        <h2>Felix the cat</h2>
    </body>
</html>
```



---
title: Step 2
files: []

---
We also need a picture of Felix, so people know what to look for. 

Images can be found in **images** folder. You have 4 images to choose from.

Now, write the `<img>` tag like you would normally, but in the src attribute, instead of writing a URL we just write images/felix-01.jpg. And don’t forget to put in an alt attribute!

```html 
<img src="images/felix-01.jpg" alt="picture of Felix">
```

##SAVE YOUR FILE AND VIEW IT IN A BROWSER.

The image is quite large, so we want to make it a bit smaller. We can do this by using height or width attributes (or both). We don’t specify the width in centimeters or meters or inches or feet, but in something called pixels. I’m going to go with 400 pixels for this image.

```html
<img src="images/felix-01.jpg" alt="picture of Felix" width="400">
```
---
title: Step 3
files: []

---
Underneath the picture we should write a description of Felix, and give some details of when and where he went missing. For this we can just write some paragraphs.

```html 
<p>Felix is a very nice cat. He likes cuddles, 
sitting in front of the radiator and his toy mouse. 
His fur is orange. </p>
<p>He went missing from the garden yesterday.</p>
```

We also need some information about how to contact the owners if anyone has seen or found Felix.

```html
<p>Have you seen Felix? 
Please contact his owners at felixowners@email.com</p>```

That’s just a pretend email address, but let’s make it so that if someone clicks on it, it opens up their email client. We do this almost the same way we make a link, but instead of a url we put in a `mailto` like this:

```html
<p>Have you seen Felix? 
Please contact his owners at 
<a href="mailto:felixowners@email.com">
felixowners@email.com
</a>
</p>
```
##SAVE YOUR DOCUMENT AND CHECK IF IT WORKS IN A BROWSER!



---
title: "Step 4: Adding strong text and emphasis"
files: []

---
We really want people to find Felix, so we want to add some *emphasis* to ‘please’. We do this with the em tag.

```html 
<p>Have you seen Felix? 
<em>Please</em> contact his owners 
at felixowners@email.com</p>
```
We also want ‘thank you’ to stand out, which we can do by adding the strong tag.

```html
<p><strong>Thank you!</strong><p>
```

##SAVE YOUR DOCUMENT AND VIEW IT IN THE BROWSER.

Notice how please is now in *italics* and Thank you is **bold**?

---
title: "Step 5: Comments"
files: []

---
Sometimes it is useful to write comments in the html file itself. By comments we mean stuff that is meant for humans to read if they’re viewing the file, and not for the browser to read and display. We do that by using the special code:

```html
<!-- write anything here -->
```

Anything between the the arrows is the comment. Let’s put a comment in our file saying this is a code club project and Felix is not real.

```html
<!-- This is a Code Club project. 
Felix is not real and not really missing -->
```

---
title: "Step 6: More metadata (that’s just stuff that goes in the head)"
files: []

---
Let’s add who wrote the webpage to the webpage, so anyone viewing the file knows it’s you.

```html
<meta name="author" content="#">
```

Replace the # with your name. It’s also common to add what language the website is in. We do this by adding an attribute to the <html> tag.

```html
<html lang="en">
```
en stands for English.

It’s also good practice to add the character set (or alphabet) the document is written in. We usually use UTF-8.

```html
<meta charset="UTF-8">
```

We can also add a description of the webpage

```html
<meta name="description" content="a page dedicated to 
finding the missing cat Felix">
```

And some keywords, separated by commas

```html
<meta name="keywords" content="Felix, cat, missing">
```
---
title: Further study
files: []

---
- Is there anything else you could add to the webpage that would help people find Felix? More information? How would you add a map of where he went missing?
- More fun with images. Add an image that moves. Try adding the image `catswithhats.gif` to the website. Open it in the browser to see what happens.
- When Felix gets found and is safely back at home, use the tag `<del>` to strike through any information that is no longer correct, like the fact that he’s missing. Use the `<ins>` tag to insert any new information instead, like Found!