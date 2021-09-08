# Frontend Mentor - Article preview component solution

## Table of contents

- [Overview](https://www.notion.so/READ-ME-Template-b07d2e3555c84e6f9291b46abf3112c6)
    - [The challenge](https://www.notion.so/READ-ME-Template-b07d2e3555c84e6f9291b46abf3112c6)
    - [Links](https://www.notion.so/READ-ME-Template-b07d2e3555c84e6f9291b46abf3112c6)
- [My process](https://www.notion.so/READ-ME-Template-b07d2e3555c84e6f9291b46abf3112c6)
    - [Built with](https://www.notion.so/READ-ME-Template-b07d2e3555c84e6f9291b46abf3112c6)
    - [What I learned](https://www.notion.so/READ-ME-Template-b07d2e3555c84e6f9291b46abf3112c6)
    - [Continued development](https://www.notion.so/READ-ME-Template-b07d2e3555c84e6f9291b46abf3112c6)
- [Author](https://www.notion.so/READ-ME-Template-b07d2e3555c84e6f9291b46abf3112c6)

## Overview

### The challenge

Users should be able to:

- Mobile friendly layout
- Animation with hover

### Links

- Solution URL: [https://github.com/mininpark/Article-preview-component](https://github.com/mininpark/Article-preview-component)
- Live Site URL: [https://article-preview-component-three-iota.vercel.app/](https://article-preview-component-three-iota.vercel.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
    - Box-shadow
    - Ballon
- Flexbox
- Click Share button for menu with jquery

### What I learned

- Positioning the element in middle of screen

    What I tried, was with position: absoulte

    **final solution: flex with justify-content and align-items**

- HTML semantic markup for important element but not to showing
- CSS custom properties
    1. Box-shadow

        ```css
        box-shadow:	0 0.125rem 0.5rem rgba(0, 0, 0, .3), 0 0.0625rem 0.125rem rgba(0, 0, 0, .2);
        ```

    2. Ballon for small triangle under the ballonbox

        ```css
        .pointer {
        	height: 20px;
        	width: 20px;
        	background: var(--font-dark-color);
        	margin: 0 auto;
            transform: rotate(225deg);
            border-radius: 0 0 12px 0;
            margin-top: -22px;
            position: relative; 
            top: 197px;
            right: 74px;
        ```

- Clicked share button for menu with jquery

    ```html
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js">
    </script>
    <script>
      $(function() {     
        $('.share_btn').on('click', function(e) {
          e.preventDefault();
          $('.share').toggleClass('hidden');
        });
      })
      </script>
    ```

### Continued development

- Styles using a pre-processor, such as Sass, Less or Stylus

## Author

- Github - [@mininpark](https://github.com/mininpark)
