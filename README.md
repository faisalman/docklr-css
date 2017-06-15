# Docklr.css

Pure CSS3 OSX-like Dock Menu & Stacks

## Usage

```html
<!-- somewhere in head -->
<link rel="stylesheet" type="text/css" href="docklr-v1.0.css" />

<!-- somewhere in body -->
<ul class="docklr">
    <li>
        <a href="index.html#mpc" id="mpc" title="Media Player">
            <img src="img/icon3-64.png" alt="" />
        </a>
    </li>
    <li>
        <a href="about.html#folder" id="folder" title="Explorer">
            <img src="img/icon1-64.png" alt="" />
        </a>
    </li>    
    <li>
        <a href="contact.html#games" id="games" title="Games">
            <img src="img/icon4-64.png" alt="" />
        </a>
    </li>
    <li>
        <a href="index.html#terminal" id="terminal" title="Terminal">
            <img src="img/icon5-64.png" alt="" />
        </a>
    </li>
    <li>
        <a href="#stack" id="stack" title="Stacks">
            <img src="img/icon2-64.png" alt="" />
        </a>
        <ul>
            <li>
                <a href="http://www.google.com" title="My Bookmarks">
                    <img src="img/icon6-64.png" alt="" />
                </a>
            <li>
                <a href="http://www.facebook.com" title="My Musics">
                    <img src="img/icon7-64.png" alt="" />
                </a>
            <li>
                <a href="http://www.twitter.com" title="My Downloads">
                    <img src="img/icon8-64.png" alt="" />
                </a>
            <li>
                <a href="http://www.yahoo.com" title="My Videos">
                    <img src="img/icon9-64.png" alt="" />
                </a>
            <li>
                <a href="http://www.apple.com" title="My Mails">
                    <img src="img/icon10-64.png" alt="" />
                </a>
        </ul>
    </li>
</ul>
```

See working example [here](https://faisalman.github.io/docklr-css). 

## Rules

* General pattern: `ul > li > [a > img ]+[ul > li > a > img]`
* The topmost `<ul>` element must have `"docklr"` class
* Tooltip will be pulled from `<a>`'s `title` attribute.
* It is recommended that `<a>`'s id match with its hash (e.g `href="contact.html#terminal"` with `id="terminal"`) so the active sign (triangle below icon) can be shown.
* `<a>`'s `href` attribute for stacks should begin with a hash (e.g `href="#stack"`)
* Image for icons must be a PNG/GIF/JPG with default size 64x64px (unless you want to modify the CSS).

## Credits

* Oxygen icon set

## License

Dual licensed under GPLv2 & MIT

Copyright © 2011 Faisal Salman <<f@faisalman.com>>

Permission is hereby granted, free of charge, to any person obtaining a copy of 
this software and associated documentation files (the "Software"), to deal in 
the Software without restriction, including without limitation the rights to use, 
copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the 
Software, and to permit persons to whom the Software is furnished to do so, 
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all 
copies or substantial portions of the Software.