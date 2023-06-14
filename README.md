 
​🇼​​🇱​​🇴​​🇦​​🇩​​🇪​​🇷​ ​🇮​​🇸​ ​🇦​ ​🇼​​🇴​​🇷​​🇰​​🇮​​🇳​​🇬​ ​🇧​​🇺​​🇮​​🇱​​🇩​​🇪​​🇷​ ​🇫​​🇴​​🇷​ ​🇭​​🇹​​🇲​​🇱​ ​🇺​​🇸​​🇮​​🇳​​🇬​ ​🇯​​🇸​​🇴​​🇳​ ​🇦​​🇳​​🇩​ ​🇯​​🇸​. 

![wloaderbanner](https://github.com/xhyabunny/wloader/assets/106491722/1eb9d4d4-086e-47f5-972e-df25340524e7)

<h1>Index</h1> 

- [Instructions](https://github.com/xhyabunny/wloader/tree/main#instructions)

- [Using the JSON file](https://github.com/xhyabunny/wloader/tree/main#using-the-json-file) > [Main indexes](https://github.com/xhyabunny/wloader/tree/main#main-indexes) > [Head & Meta elements](https://github.com/xhyabunny/wloader/tree/main#head--meta-elements) > [The modifiers](https://github.com/xhyabunny/wloader/tree/main#the-modifiers) > [OnLoad animations](https://github.com/xhyabunny/wloader/tree/main#onload-animations)
- [Credits](https://github.com/xhyabunny/wloader/tree/main#credits)

<h1>Instructions</h1> <img style="
  height: 40px;width: 40px;" src="https://github-production-user-asset-6210df.s3.amazonaws.com/106491722/245261475-f581fca3-0ed6-4f8e-9385-1af112c3d46b.png"
  />

This package will come with 2 scripts. 

``wloader.js``
``wloader.json``
 ᵁˢᵘᵃˡˡʸ ʸᵒᵘ ʲᵘˢᵗ ᵘˢᵉ ᵗʰᵉ ᴶˢᴼᴺ

🔹 You can implement them on your code just drag & dropping these two into your project:

<img style="
  height: 170px;width: 270px;" src="https://github-production-user-asset-6210df.s3.amazonaws.com/106491722/245296091-62f1f928-582e-4541-abda-a0b30dca8eb9.png"
  />
 
🔹 And then accessing the JS script through HTML using the ``<script>`` tag in any part of your code:

```html
<script src="./path/to/wloader.js"></script>
```

✔ *You can also recycle this script globally in another HTML file just calling the script with its respective tag like shown above!*

✔ *If you're willing to modify anything to your likings on the JS script, you are welcomed to do so, as long as you know what you're doing.
You could even create an issue and suggest things to be added!*

## Using the JSON file

The first thing to see when you open the JSON file, is probably going to look very odd or messy, tabulation was made specifically for it to be as organized as possible
for your mind to be able to read it properly, so lets check out a few things about this JSON file.

<h3>Main indexes</h3>

The first thing you will realize when you check this json file, are both the ``html`` and ``css`` indexes:

```json
"html": "./index.html",
"css": "./index.css",
```

❕ Those are to be replaced with the actual paths to both your *main css index* and your *main html index*

⚠ *It's VERY IMPORTANT that you add the two main indexes, if you ever need to add another CSS file, you can add these on each respective array, we'll get to that soon.*

<h3>Head & Meta elements</h3>

The head and meta values on your JSON file by default will will look like this:

```json
    "head": 
    {
        "title": "wloader",
        "icon": "https://github-production-user-asset-6210df.s3.amazonaws.com/106491722/245261475-f581fca3-0ed6-4f8e-9385-1af112c3d46b.png",
        "meta": [ "og:title \\ wloader-app",
            "og:description \\ WLoader is a working and reusable script that builds a simpler HTML using JSON and JS.",
                    "og:url \\ https://xhyabunny.com/wloader",
                  "og:image \\ https://github-production-user-asset-6210df.s3.amazonaws.com/106491722/245261475-f581fca3-0ed6-4f8e-9385-1af112c3d46b.png",
            "og:theme-color \\ #000000",
                  "viewport \\ width=device-width, initial-scale=1, minimum-scale=1.0",
                    "length \\ 6" ],
        "meta_embed_image": false
    },
```

This part of the JSON file contains the info about the Webpage icon, title and its embedding on social media.

Notice the ``length`` key, which is valued ``6``, this number is the quantity of meta links that are in the list ``(excepting itself)``, if you ever wanted to add another element to the array, please maintain the ``length`` value according to the quantity of lines that the array contains.

Notice the separation of each string with ``\\`` character, which marks the relative key ``(left side)`` and value ``(right side)`` of each string as if it was a normal json variable.

You wanna change the value of each key with the information you want, as long as your inserted value is correct and according to each meta link and you respect the assigned order given to you (``"key\\value"``).

As for ``meta_embed_image`` boolean, if set to ``true``, your ``og:image`` element will become a big cover image, instead of just a tiny logo at the side of your embed. 

🔸 Here's an example:

<img style="
  height: 550px;width: 590px;" src="https://github-production-user-asset-6210df.s3.amazonaws.com/106491722/245301592-37c9eb5a-5287-43ba-95b8-745c4c38ff09.png"
  />
  
<h3>The modifiers</h3>

Modifiers look something like this:

```json
"sample": "modifier1\\modifier2\\content"
```

They are ordered and we'll call them:

```json
"KEY": "ATTRIBUTE_MODIFIER\\TYPE_MODIFIER\\TARGET_VALUE"
```

Again notice how its separated by ``\\``

They are used to implement several features on each element of the HTML, for example, if we wanted a script to have the ``module`` type
we could just change our type modifier to one of our scripts.

```json
"scripts": [
  "module\\null\\.path/to/script.js"
]
```

If you don't need to use these modifiers you can just tag them with ``null``.

And then for attributes we can add them like this:

```json
"scripts": [
  "module\\defer\\.path/to/script.js"
]
```

As for attribute modifiers, you can add as many attributes you want as long as you separate them with a space in between.

Now your script will load as a module typed script, and with its defer attribute

⚠ *REMEMBER: MODIFIERS GO IN ORDER, YOU CAN'T PUT TYPE MODIFIERS INSIDE ATTRIBUTE MODIFIERS AND/OR THE OTHER WAY AROUND*

This also happens with links, but to resume it; 

The first modifier changes the ``rel`` type of link you are implementing to the ``<head>`` element, for example:
- ``stylesheet``
- ``preconnect``
- ``etc``

The next modifier is attributes, same logic as scripts, for example:
- ``crossorigin``
- ``etc``

The target value would be the ``content`` tag of this link, which is up to you.

<h3>OnLoad animations</h3>

These are animations that progressively transition the opacity of your whole page from 0 to 1.

You can change them here:

```json
"animationType": "fast",
```

It is set to ``fast`` by default, but you have many options:
- ``none`` (disabled)
- ``faster``
- ``fast``
- ``smooth``
- ``smoother``

All of them define a faster or slower entry transition.

## Credits

- xhyabunny
- sanicbtw (recycled idea)
