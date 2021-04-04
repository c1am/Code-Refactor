# 01 HTML, CSS, and Git: Code Refactor Homework

# Purpose of the Assignment
```
The purpose of the assignment was to refactor the code of a marketing agency website without changing what it does and make sure that the website meets the correct accessbility standards.
```

# Changes to index.html
```
Changed the div in `<div class="header">`, to just `<header>` since 'header' is a semantic HTML element on its own, no need for the extra `div` and then `class` elements.

Changed the second div to `<nav>` since it seems most like a navigation bar within the header.

Changed div in `<div class="hero"></div>` to `<figure class="planning image" alt="People meeting around a conference room table."></figure>` as it is a self-contained image and added the alt for accessibility.

Changed div in `<div class="content">` to `main` because it will contain the most important and biggest part of the page.

Changed the three divs nested under `class=content` to `article` because those three sections are each their own but together make up the main/most important portion of the website.

Added `alt` to all three images nested under the three articles in the main for accessibility.

Changed the div in the right pane to `<aside>` because the panel is its own container to the side of the main content.

Changed the three divs immediately under the `benefits` class to `<section>` because while they are their own containers, they are still just sections in the same aside element.

Added `alt` to all three images nested under the three sections in the `aside` for accessibility.

Changed the div in `<div class="footer">` to just `<footer>` because there is no need to put both div and class if footer is an element of its own.
```

# Changes to style.css
```
Changed the `class` and `id` elements to the respective semantic element changes in index.html.
* i.e: header, nav, .planning-image, section, article, footer

Condensed a lot of the repetitive stylings under one overarching parent into one for a cleaner code.
* i.e: Combined `.search-engine-optimization h2 {...}`, `.online-reputation-management h2 {...}`, and `.social-media-marketing h2 {...}` into `.content article h2 {...}` because the styles of these three equal elements were the same.

Changed the background color of the side panel to a little darker / almost same as background color of main content to provide a more suitable contrast in accordance to accessbility standards. *Inspect Lighthouse feature was used to measure accessibility.*
```