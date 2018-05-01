# startpage

a startpage is the page you first see when you open your browser. by default your browser will usually show you a built-in "new tab" page, or your homepage (if defined). i wanted to rely less on browser based bookmarks and create my own method to quickly access my most commonly viewed linx. typing in the search box (with the all seeing eye) will live filter the results and reveal hidden linx. use `tab` then `enter` to select and navigate to urls. the default submit action on the searchbox will send your query to google (this easily overridden to the search engine of your choice by adjusting the form action value).

## preview (nord theme)

![startpage preview](https://gist.githubusercontent.com/xero/cbcd5c38b695004c848b73e5c1c0c779/raw/17a66428a511943ccf80d9ed4d21a2b694f57ccf/start-page-preview.png)

## goals

* create a personalized startpage
* all assets (fonts, images, css, etc) are embedded directly into the source
* responsive sizing
* keyboard-centric ui
* dynamically searchable
* support for hidden linx (that reveal on search)
* easily hosted and updated (either locally or remotely)

## files

* startpage.html - the main project implementation
* startpage-nord.html - a colorscheme variant inspired by [nord](https://arcticicestudio.github.io/nord/)
* startpage-static.html - the non-javascript version

## notes

this targets the newest version of chromium, since that's what i use (with some of the [inox patches](https://git.io/inox)). i've also tested against the newest firefox and it should work fine with other modern browsers.

if you plan to use this file locally, you'll need the [new tab redirect](https://goo.gl/cew899) extension. use the `file:///home/x0/dotfiles/startpage.html` address syntax.

the font base64 encoded and embedded into the source is the classic amiga font [topaz](https://trueschool.se/html/fonts.html) - more download options are available [here](https://github.com/rewtnull/amigafonts).

these are not (all) the bookmarks i actually use. i tried to amass a nice large collection for demo purposes.

since there are no external libs, i used `$` to define my dom manipulation functions and `_` for the link library. if you plan to fork and extend this with either jquery or underscore.js please take note.

## license

![kopimi logo](https://gist.githubusercontent.com/xero/cbcd5c38b695004c848b73e5c1c0c779/raw/6b32899b0af238b17383d7a878a69a076139e72d/kopimi-sm.png)

[kopimi](https://kopimi.com)! in the spirit of _freedom of information_, i encourage you to fork, modify, change, share, or do whatever you like with this project! `^c^v`
