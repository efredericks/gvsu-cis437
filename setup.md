---
layout: page
title: Setup Guide
description: >-
    Setup Guide page.
---

# Setup Guide(s)

{:.no_toc}

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

This page lists out the setup guides for the tools used in class - the tricky one will be Three.js.  

---

All you need for this class is a text editor and a modern browser. I will be using VSCode and Chrome (Firefox has been laggy lately with WebGL for some reason), however feel free to use whichever WebGL-enabled browser you wish. If you are looking for a modern IDE that supports JavaScript, consider VSCode, JetBrains (should be free via student educational discount), or Brackets.

## Angel libraries (local)

Here is the [book's webpage](https://www.cs.unm.edu/~angel/BOOK/INTERACTIVE_COMPUTER_GRAPHICS/SEVENTH_EDITION/){:target="\_blank"}.  You can directly get the library files from the [GitHub page](https://github.com/esangel/WebGL/tree/master/Common){:target="\_blank"}.

You mainly just need to ensure that your libraries are in a common location to all your other files and are easily referenced.  If you wish you can run a local web server, though that is only necessary if you are loading in assets.  In this case, you can add the [Live Server extension to VSCode](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer){:target="\_blank"} (what I use). 

Alternatively, you can use Python's built-in web server by calling:

`python3 -m http.server`

This assumes that Python is installed, is referenced as `python3`, and that you're calling it on your local terminal.  See [this page](https://docs.python.org/3/library/http.server.html){:target="\_blank"} for details.  By default, it will run on port 8000.

You could also try [WAMP](https://www.wampserver.com/en/){:target="\_blank"} or [MAMP](https://www.mamp.info/en/downloads/){:target="\_blank"} as well, if you want to install a program for Windows or Mac, respectively.

**Regardless**, you'll need to setup your folder structure to reference the libraries.  I recommend a structure like this:

```
+ CIS367
  + libraries
    + Common
      - MV.js
      - MV2.js
      - README.txt
      - initShaders.js
      - initShaders2.js
      - webgl-utils.js  
  + hw1
    - hw1-mylastname.html
    - hw1-mylastname.js
  + hw2
    - hw2-mylastname.html
    - hw2-mylastname.js
  ...
```

Now, if you're editing hw1-mylastname.html, it should look like this:

```html
<!DOCTYPE html>
<html>
  <meta http-equiv="Content-Type" content="text/html;charset=utf-8" >
  <title>HW title</title>

  <script id="vertex-shader" type="x-shader/x-vertex">
    // vertex shader code
  </script>

  <script id="fragment-shader" type="x-shader/x-fragment">
    // fragment shader code
  </script>

  <script type="text/javascript" src="../libraries/Common/webgl-utils.js"></script>
  <script type="text/javascript" src="../libraries/Common/initShaders.js"></script>
  <script type="text/javascript" src="../libraries/Common/MV.js"></script>
  <script type="text/javascript" src="hw1-mylastname-script.js"></script>
</head>
...
</html>
```

You *should* be able to just open `hw1-mylastname.html` directly in your browser.

### Boilerplate Download

Here is a link to a boilerplate download you can use.  Note that I follow the directory structure above.

[Boilerplate setup](/assets/CIS367.zip)

## Three.js (local)

There are two main considerations when running three.js locally.  

1. If you are loading in any objects, materials, sounds, pictures, etc., you **will need** to run a local web server.
  - Run a local web server and view the site on whatever port you're running it on (e.g., http://localhost:8888)

2. If you are **not loading** anything in separately, you **do not need** to run a local web server.
  - Just open the HTML file locally in your browser (e.g., file://path/to/your/file.html)

This occurs because of cross-site scripting protection that browsers enact to keep you safe (mainly to avoid malicious web sites from loading in things that shouldn't be loaded).  Most of what we'll be doing will be (2) - no web server needed.  You write your JavaScript/shader code and just open the HTML file in your browser.

**Note**: you will need to move your code to a public web server (e.g., your EOS web space, GitHub pages, etc.) for grading and/or sharing.

### Lessons Learned (gotchas)

1. Get comfortable with your browser's developer tools. All your JavaScript errors (i.e., your application errors) will show up in the console.  Usually you'll have a very helpful error message that tells you what is wrong.  
  * Google Chrome: Menu -> More Tools -> Developer Tools (Ctrl+Shift+I) 
  * Mozilla Firefox: Settings -> More Tools -> Web Developer Tools (Ctrl+Shift+I)
  * Edge / Safari / Opera / Netscape: You're on your own.

2. When writing shaders, all of your compilation errors will show up as a popup when you load the page.  They're not always helpful, but should hopefully give you an indication as to what is wrong.

3. If you are not seeing anything in your scene, you might be:
   * Missing a light
   * Missing a camera
   * Pointing your camera in the wrong direction
   * Having an error message (did you check your console?)

4. If you are expecting textures to show up on your objects but they are black or otherwise weird-looking, you probably forgot to start your web server.

## Blender

Download the [Blender installer](https://www.blender.org/download/){:target="_blank"} and install as specified.  This software is open source and free.

## Unity

Download the [Unity installer](https://store.unity.com/#plans-individual){:target="_blank"} and install as specified.  Note - you'll need to sign up for a **Student** account.  This is free as long as you're not making a specific amount of money on your projects.
