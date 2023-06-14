
​🇼​​🇱​​🇴​​🇦​​🇩​​🇪​​🇷​ ​🇮​​🇸​ ​🇦​ ​🇼​​🇴​​🇷​​🇰​​🇮​​🇳​​🇬​ ​🇧​​🇺​​🇮​​🇱​​🇩​​🇪​​🇷​ ​🇫​​🇴​​🇷​ ​🇭​​🇹​​🇲​​🇱​ ​🇺​​🇸​​🇮​​🇳​​🇬​ ​🇯​​🇸​​🇴​​🇳​ ​🇦​​🇳​​🇩​ ​🇯​​🇸​. 

![wloaderbanner](https://github.com/xhyabunny/wloader/assets/106491722/1eb9d4d4-086e-47f5-972e-df25340524e7)


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
 
🔹 And then accessing the JS script through HTML using the ``<script>`` tag in any part of your code, always in the main index file:

```html
<script src="./path/to/wloader.js"></script>
```

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

⚠ *It's VERY IMPORTANT that you add the two main indexes, not all of the other files, if you ever need to add another HTML or CSS file, you can add these on each respective array, we'll get to that soon.*

<h3>Head & Meta elements</h3>

The head and meta values on your JSON file by default will will look like this:

```json
    "head": 
    {
        "title": "wloader",
        "icon": "https://github-production-user-asset-6210df.s3.amazonaws.com/106491722/245261475-f581fca3-0ed6-4f8e-9385-1af112c3d46b.png",
        "meta": [ "og:title \\ wloader-app",
            "og:description \\ WLoader is a working head-builder for HTML using JSON and JS",
                    "og:url \\ https://xhyabunny.com/wloader",
                  "og:image \\ https://github-production-user-asset-6210df.s3.amazonaws.com/106491722/245261475-f581fca3-0ed6-4f8e-9385-1af112c3d46b.png",
            "og:theme-color \\ #000000",
                  "viewport \\ width=device-width, initial-scale=1, minimum-scale=1.0",
                    "length \\ 6" ],
        "meta_embed_image": false
    },
```

This part of the JSON file contains the info about the Webpage icon, title and its embedding on social media.

<p>Notice the separation of each strings with the ``\\`` character, which marks the key *(left side)* and the value *(right side)* of each string.
You wanna change the value of each key with the information you want, as long its valid for each object and you respect the assigned order.</p>

As for ``meta_embed_image`` boolean, if set to ``true``, your ``og:image`` element will become a big cover image, instead of just a tiny logo at the side of your embed. 

🔸 Here's an example:

<img style="
  height: 550px;width: 590px;" src="https://github-production-user-asset-6210df.s3.amazonaws.com/106491722/245301592-37c9eb5a-5287-43ba-95b8-745c4c38ff09.png"
  />
  
<h3>The modifiers</h3>
