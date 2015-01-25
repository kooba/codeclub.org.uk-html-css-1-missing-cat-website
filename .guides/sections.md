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


---
title: Example section 4
editable: true

---
Some **awesome** content 4
