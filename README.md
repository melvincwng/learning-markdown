# Learning Markdown

A repository where I document my process of learning the Markdown language

## What is Markdown?

Markdown is a lightweight markup language that converts text to HTML. In short, it helps to format text that appear on the screen.

## Why am I learning Markdown?

To improve my proficiency in the **JAM stack** (JavaScript, APIs, Markup). It is a tech stack where the application logic typically resides in the client side, without being tightly coupled to the backend server.

## What is Markdown used for?

1. Readme Files (e.g. Github)
2. Forum & Blog posts
3. Used in many Static Site Generators (e.g. Gatsby, Hugo, Jekyll)

## Syntax of Markdown

<!-- Able to use HTML code/comments in .md files also -->

**A) Core Markdown syntax**

1. Headings

   # H1 header

   ## H2 header

   ### H3 header

   #### H4 header

   ##### H5 header

   ###### H6 header

2. Italics - Can use \* \* or \_ \_

   _This text is italic_

3. Strong - Can use \*\* \*\* or \_\_ \_\_

   **This text is bold**

4. Strikethrough - Can use ~~ ~~

   ~~This text is strikethrough~~

5. Horizontal Rule (a horizontal line), can use triple --- or \_\_\ or \*\*\*

   ***

6. Escape character: \ (backslash)

7. Blockquote: Use >

   > This is a quote

8. Links - a) [text goes here](link goes here) **OR** b) [text goes here](link goes here space insert_title)

   a) [Markdown Guide](https://www.markdownguide.org/)
   b) [Markdown Guide](https://www.markdownguide.org/ "Hover over to see title")

9. UL - Insert a \- or \* for each item

   - Item 1
   - Item 2
   - Item 3
     - Nested Item 1 (insert tabs)
     - Nested Item 2

10. OL

    1. Item 1
    1. Item 2
    1. Item 3

11. Inline Code Block - Use backticks ``

    e.g. This is an `inline code block`. Notice it's color is different from the rest of the words.

12. Images - ![text](image link)

    Normal image using Markdown syntax (can't adjust width & height)
    ![Twitter Logo](https://icon-library.com/images/small-twitter-icon/small-twitter-icon-9.jpg)

    Alternative image (using HTML code - can adjust width & height)
    <img src="https://icon-library.com/images/small-twitter-icon/small-twitter-icon-9.jpg" width="100px" height="100px">

**B) Github Markdown syntax (Github has their own flavor of using Markdown)**

1. Code Blocks (in GitHub) - Use triple backticks \`\`\` \`\`\`

   ```
   npm install

   npm run start
   ```

   Provides special highlighting

   ```javascript
   function add(num1, num2) {
     return num1 + num2;
   }
   ```

2. Tables

   | Name | Email          |
   | ---- | -------------- |
   | John | john@gmail.com |
   | Doe  | doe@gmail.com  |

3. Task lists (should show up as checkboxes in Github README.md)

   - [x] Task 1
   - [x] Task 2
   - [ ] Task 3

4. Note there's also online 'Markdown to HTML code' converters online that convert your Markdown code to HTML code (in case you want to see how it looks like in HTML):

   - https://markdowntohtml.com/

## References

1. Markdown Crash Course [Traversy Media] - https://youtu.be/HUBNt18RFbo
2. https://www.markdowntutorial.com/lesson/1/
3. https://www.markdownguide.org/
4. https://en.m.wikipedia.org/wiki/Jamstack
5. https://blog.dreamfactory.com/the-importance-of-loose-coupling-in-rest-api-design/
