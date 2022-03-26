# Learning Markdown

A repository where I document my process of learning the Markdown language

## What is Markdown?

Markdown is a lightweight markup language that converts text to HTML. In short, it helps to format text that appear on the screen.

## Why am I learning Markdown?

To improve my proficiency in the **JAM stack** (JavaScript, APIs, Markup). It is a tech stack where the application logic typically resides in the client side, without being tightly coupled to the backend server.

## JAM stack architecture vs Traditional Web architecture

**Traditional Web**: Client <--> Server <--> Database/CMS

**JAM stack**:

Based on my understanding, what is JAM stack:

- Static Site Generators like Gatsby/Hugo/Jekyll generate the static HTML/CSS/JS files of your website based on A) your **input files** & B) a set of **template files**:
  - **Input files**: a) Files that provide the data/content of your website - e.g. Markdown files (which will later be converted to HTML files using the SSG) AND b) Other types of static files - e.g CSS/JS/Image files
  - **Template files**: Derived from the templating engine used in the SSG - e.g. Gatsby uses React as it's templating engine.
  - For more information, can visit the Youtube video link **(reference 7)** & Gatsby repo link **(reference 8)** below to see how the markdown, css, js and image files are organized in a Gatsby-generated site.
- These pre-built static HTML/CSS/JS files are then hosted on a CDN, which are served to users when requested.
- Since they are pre-built, they load very quickly in users' browsers. The static content is first shown to the user (M portion).
- Next, the javascript code in the JS files executes in the client/browser (J portion) to handle some logic. For instance, the JS code executes to call API endpoints (A portion) to fetch dynamic content.
- The dynamic content will then be fetched from the API endpoint & then be shown to the user (both static + dynamic content shown to the user now in your website).

**Useful images for visualization**
<br />
<span>
<img src="https://d33wubrfki0l68.cloudfront.net/b7d16f7f3654fb8572360301e60d76df254a323e/385ec/img/svg/architecture.svg" width="400px" height="300px"/>
<img src="https://devopedia.org/images/article/78/9117.1525882869.jpg" width="400px" height="300px">
<img src="https://www.fullstackpython.com/img/visuals/pelican-flow.jpg" width="400px" height="300px">
<img src="https://uploads.toptal.io/blog/image/126943/toptal-blog-image-1534876856505-558f1c71902d47812f218825d358fe4b.png" width="400px" height="300px">
<img src="https://bejamas.io/static/1b59935d7ad1796f1c6373d45ba31b76/05035/ssg--intro-1--light.png" width="400px" height="300px">
<img src="https://bejamas.io/static/5e89ac2073c9fc3286c7d284b04e5196/07564/ssg--intro-2--light.png" width="400px" height="300px">
</span>

References:

    [1] https://jamstack.org/
    [2] https://www.fullstackpython.com/static-site-generator.html
    [3] https://www.cloudflare.com/en-gb/learning/performance/static-site-generator/
    [4] https://bejamas.io/discovery/static-site-generators/
    [5] https://www.toptal.com/front-end/static-site-generators-comparison-2018
    [6] https://devopedia.org/static-site-generators
    [7] Gatsby Markdown Tutorial: https://www.youtube.com/watch?v=rgyTpQVDP44
    [8] Gatsby-generated Website Source Code: https://github.com/guidingdigital/yt-gatsby-markdown

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

3. Bold - Can use \*\* \*\* or \_\_ \_\_

   **This text is bold**

4. Bold & Italic - Can use \*\*\* \*\*\*

   **_This text is both bold & italic_**

5. Strikethrough - Can use ~~ ~~

   ~~This text is strikethrough~~

6. Horizontal Rule (a horizontal line), can use triple --- or \_\_\ or \*\*\*

   ***

7. Escape character: \ (backslash)

8. Blockquote: Use >

   > This is a quote

9. Links - a) [text goes here](link goes here) **OR** b) [text goes here](link goes here space insert_title)

   a) [Markdown Guide](https://www.markdownguide.org/)
   b) [Markdown Guide](https://www.markdownguide.org/ "Hover over to see title")

10. UL - Insert a \- or \* for each item

- Item 1
- Item 2
- Item 3
  - Nested Item 1 (insert tabs)
  - Nested Item 2

11. OL

    1. Item 1
    1. Item 2
    1. Item 3

12. Inline Code Block - Use backticks ``

    e.g. This is an `inline code block`. Notice it's color is different from the rest of the words.

13. Images - ![text](image link)

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
5. https://jamstack.org/
6. https://blog.dreamfactory.com/the-importance-of-loose-coupling-in-rest-api-design/
