# Purpose

I plan to move the theme [pelican-elegant](https://github.com/talha131/pelican-elegant/) from bootstrap to postcss. Unfortunately a lot of styles used in the theme are dependent on the specific version of the bootstrap I used, which makes it hard to maintain.

I intend to use this repository to extract relevant CSS rules and use it as a rebirth of the Pelican Elegant theme.

For example, 

1. I want to figure what CSS rules are in use to display top navigation menu as it is
1. Remove all the code from `<body>` of index.html but leave top navigation menu code
1. Run `npm run uncss -- index > menu.css`. 

It will place all the rules used in index.html in menu.css file. As we have removed everything but the menu from the index.html, menu.css will only contain the rules that are used for navigation menu.

# Commands

1. `npm run server` to view website in browser
1. `npm run uncss -- <filename>` to run uncss on a file
