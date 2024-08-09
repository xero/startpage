# startpage

a startpage is the page you first see when you open your browser. by default your browser will usually show you a built-in "new tab" page, or your homepage (if defined). i wanted to rely less on browser based bookmarks and create my own method to quickly access my most commonly viewed linx. typing in the search box (with the all seeing eye) will live filter the results and reveal hidden linx. use `tab` then `enter` to select and navigate to urls. the default submit action on the searchbox will send your query to google (this is easily overridden to the search engine of your choice by adjusting the form action value). the search box also features `!bang` syntax to search different providers (e.g. google, github, shodan, greynoise, etc).

## preview (nord theme)

![startpage preview](https://gist.githubusercontent.com/xero/cbcd5c38b695004c848b73e5c1c0c779/raw/17a66428a511943ccf80d9ed4d21a2b694f57ccf/start-page-preview.png)

## !bangs

prepend your search with a supported `!bang` to search somewhere other that google.

 * `!a` amazon product search
 * `!bc` bandcamp search
 * `!e` ebay search
 * `!gh` github code search
 * `!gn` greynoise query
 * `!h` http status code docs
 * `!i` google images search
 * `!s` shodan snooping
 * `!t` google translate
 * `!w` wikipedia search
 * `!y` youtube search
 * `!yh` youtube history search

## features

* create a personalized startpage
* all assets (fonts, images, css, etc) are embedded directly into the source
* responsive sizing
* keyboard-centric ui
* dynamically searchable
* support for hidden linx (that reveal on search)
* easily hosted and updated (either locally or remotely)

## files

* startpage.html - the main project implementation
* startpage-static.html - the non-javascript version

## notes

[homepage for safari](https://apps.apple.com/gb/app/homepage-for-safari/id6481118559) and [new tab redirect for chrome](https://goo.gl/cew899) are the new tab extensions i've tested. if you plan host the startpage locally, use the `file:///home/x0/dotfiles/startpage.html` address syntax.

the font base64 encoded and embedded into the source is the free/open source [hack](https://github.com/blinksh/patched-fonts/blob/5fb174fb75987e735fda8f0643fd76911f21fa97/Hack%20Nerd%20Font.css) patched from the nerd fonts collection.

these are not `{all,}` the bookmarks i actually use. i tried to amass a nice large collection for demo purposes to showcase it's dynamic sizing, and shoutout some friends!

since there are no external libs, i used `$` to define my dom manipulation functions and `_` for the link library. if you plan to fork and extend this with either jquery or underscore.js please take note. _but ewww gross._

## license

![kopimi logo](https://gist.githubusercontent.com/xero/cbcd5c38b695004c848b73e5c1c0c779/raw/6b32899b0af238b17383d7a878a69a076139e72d/kopimi-sm.png)

[kopimi](https://kopimi.com)! in the spirit of _freedom of information_, i encourage you to fork, modify, change, share, or do whatever you like with this project! `^c^v`
