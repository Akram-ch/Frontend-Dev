# Responsive Design Course notes

Personal Token key : 
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

## I - Cat Photo app : 
### HTML attributes :
An HTML attribute is a piece of markup language used to adjust the behavior or display of an HTML element. For example, attributes can be used to change the color, size, or functionality of HTML elements.
###  images
* img is a self closing tag
* HTML attributes are special words used inside the opening tag of an element to control the element's behavior
* The src **attribute** in an img element specifies the image's URL (where the image is located)
* The alt attribute's text is used for screen readers to improve accessibility and is displayed if the image fails to load
* You can link to another page with the anchor (a) element
* `<a href='https://freecodecamp.org'></a>`

### Anchors 
* `<a href='https://github.com/'> </a>`
* `targe = "_blank"` ==> open in new tab
  
### Lists
#### ***Unordered Lists***
* `<ul></ul>`
* ```html
    <ul>
        <li>milk</li>
        <li>cheese</li>
    </ul>
    ```

### Figure :
The figure element represents self-contained content and will allow you to associate an image with a caption.

### Figure Caption :
A figure caption (figcaption) element is used to add a caption to describe the image contained within the figure element.
```html
    <figure>
        <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
        <figcaption> Cats love lasagna. </figcaption>
    </figure>
```
### Emphasis
  `<em>love</em>` -->  <em>love <em>


### Forms
```html
<form action="/ma-page-de-traitement" method="post">
    <div>
        <label for="name">Nom :</label>
        <input type="text" id="name" name="user_name">
    </div>
    <div>
        <label for="mail">e-mail&nbsp;:</label>
        <input type="email" id="mail" name="user_mail">
    </div>
    <div>
        <label for="msg">Message :</label>
        <textarea id="msg" name="user_message"></textarea>
    </div>
</form>
```

* Define min and max values :  
      `<input type="number" id="tentacles" name="tentacles"
       min="10" max="100">`
* add placeholder text : 
Email: <input type="text" name="email" `placeholder="Email"/><br><br>`

#### **Drop down menu** : 
<label for="pet-select">Choose a pet:</label>
```html
<select name="pets" id="pet-select">
    <option value="">--Please choose an option--</option>
    <option value="dog">Dog</option>
    <option value="cat">Cat</option>
    <option value="hamster">Hamster</option>
    <option value="parrot">Parrot</option>
    <option value="spider">Spider</option>
    <option value="goldfish">Goldfish</option>
</select>

```
#### **Radio buttons**
```   html
 <legend>Select a maintenance drone:</legend>

    <div>
      <input type="radio" id="huey" name="drone" value="huey"
             checked>
      <label for="huey">Huey</label>
    </div>

    <div>
      <input type="radio" id="dewey" name="drone" value="dewey">
      <label for="dewey">Dewey</label>
    </div>

    <div>
      <input type="radio" id="louie" name="drone" value="louie">
      <label for="louie">Louie</label>
    </div>
</fieldset>
```

#### **Checkboxes**
``` html
<fieldset>
    <legend>Choose your monster's features:</legend>

    <div>
      <input type="checkbox" id="scales" name="scales"
             checked>
      <label for="scales">Scales</label>
    </div>

    <div>
      <input type="checkbox" id="horns" name="horns">
      <label for="horns">Horns</label>
    </div>
</fieldset>
```

### **Text Areas**
```html
<label for="story">Tell us your story:</label>

<textarea id="story" name="story"
          rows="5" cols="33">
It was a dark and stormy night...
</textarea>
```
### **Submit button**
`<input type="submit" value="Envoyer le formulaire">`

### Link external style sheet
   int the head section :  
    `<link rel="stylesheet" href="styles.css">`

___
## CSS : Box Model
In the CSS box model, every HTML element is treated as a box with four areas.

Imagine you receive a box from your favorite online retailer -- the content is the item in the box, or in our case, a header, paragraph, or image element.
The content is surrounded by a space called padding, similar to how bubble wrap separates an item from the box around it.

Think of the border like the cardboard box your item was shipped in.
Margin is the area outside of the box, and can be used to control the space between other boxes or elements.

![screenshot](./css.png)

#### to round off edges:   `border-radius : 10px;`


### Dynamic boxes : `  width: calc(25% - 20px);`
___
## CSS FLEXBOX : Image Gallery:

Flexbox is a one-dimensional CSS layout approach that focuses on the flow of content. It offers the ability to control the way items are spaced and aligned within a container.

To set an element to use Flexbox, you give it a display property set to flex

Flexbox can be thought of as having two axes, the **main axis** and the **cross axis**. The main axis is determined by the **flex-direction** property. If flex-direction is set to **row** or **row-reverse**, the main axis is horizontal. If flex-direction is set to **column** or **column-reverse**, the main axis is vertical.

The **flex-wrap** property determines how your items should behave when the flex container is too small. Setting this property to **wrap** will allow your items to wrap to the next row/column (depending on your main axis), where **nowrap** will prevent your items from wrapping. When this is set to nowrap, items may either shrink to fit or overflow.

The **justify-content** property determines how the items inside a flex container are positioned along the __main axis__, affecting their position and the space around them.

The **align-items** property positions the flex content along the __cross axis__. In this case, with your flex-direction set to row, your cross axis would be vertical.

you can use the **object-fit** property to determine how images should behave.

### Flex properties: 
* **flex-start**: Items align to the left side of the container.
* **flex-end**: Items align to the right side of the container.
* **center**: Items align at the center of the container.
* **space-between**: Items display with equal spacing between them.
* **space-around**: Items display with equal spacing around them.
* **row**: Items are placed the same as the text direction.
* **row-reverse**: Items are placed opposite to the text direction.

## CSS : Typography
**import open sans font-family** : 
``` html
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Open+Sans:400,700,800">
```

``` css
  font-family: "Open Sans", sans-serif;
  ```

**font size** : 
``` css
font-size: 16px;
```

**make text bolder**: 
``` css
  font-weight: 800;
```
**align text**: 
```css
text-align: center;
```
**top and bottom margin of -4px and a left and right margin of 0** : 
``` css
margin: -4px 0;
```
### The letter-spacing property can be used to adjust the space between each character of text in an element.
```css
  letter-spacing: 0.15px;
```
### The **float** property is used to place an element on the left or right of its container, allowing other content (such as text) to wrap around it.


### The **rem** unit stands for **root em**, and is relative to the font size of the **html** element.

### avoid overflows :
```CSS
overflow: hidden;
```

### **clear** property, lear the float property, pushing the divider and any following content down below the float text

___

## Intermediate HTML and CSS
### Default styles :
* [The Meyer reset](https://meyerweb.com/eric/tools/css/reset/)
* [normalize.css](https://nicolasgallagher.com/about-normalize-css/)

### CSS Units : 
 * #### absolute units:
    Absolute units are those that are always the same in any context. px is an absolute unit because the size of a pixel doesn’t change relative to anything else on the page. In fact, px is the only absolute unit you should be using for web projects. The rest of them make more sense in a print setting because they are related to physical units such as in (inch) and cm (centimeter).
* #### Relative units :
    em and rem both refer to a font size, though they are often used to define other sizes in CSS. You’ll see both of them often so we’re going to explain both, but as a rule-of-thumb, prefer rem.

  1em is the font-size of an element (or the element’s parent if you’re using it to set font-size). So, for example, if an element’s font-size is 16px, then setting its width to 4em would make its width 64px (16 * 4 == 64).

  1rem is the font-size of the root element (either :root or html). The math works the same with rem as it did with em, but without the added complexity of keeping track of the parent’s font size. Relying on em could mean that a particular size could change if the context changes, which is very likely not the behavior you want.

  Using a relative size like rem to define font sizes across your website is recommended. Many browsers allow users to change the base font-size to increase readability. If at all possible, it is advisable to respect a user’s wishes regarding font size. You’ll learn more about this from the reading assignments.
* #### Viewport units :
    The units vh and vw relate to the size of the viewport. Specifically, **1vh** is equal to 1% of the viewport height and **1vw** is equal to 1% of the viewport width. These can be useful any time you want something to be sized relative to the viewport, examples including full-height heroes, full-screen app-like interfaces.


[article](https://codyloyd.com/2021/css-units/)

### Fonts : 
* #### The system font stack : 
    If you use the font-family property to change to a font like impact or Times New Roman, and those fonts do not happen to be installed on your user’s computer, then a fallback font will be displayed. If you have not defined a fallback, then the default HTML font will be used, which is often somewhat ugly. For this reason, it’s common to see somewhat long stacks of fonts listed on projects.
``` CSS
body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
}
```
#### Online font libraries : 
[Google Fonts](https://fonts.google.com/)

[Font Library List](https://fontlibrary.org/)

[Adobe Fonts](https://fonts.adobe.com/)
    
  To use a font from one of these libraries, go to the website, select a font and then copy a snippet from the website to import that font from their server into your website. You’ll be given either a < link > tag to put in your HTML like so….
  ``` css
  <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">
```
 or an @import tag that can be dropped at the top of a CSS file
 ``` CSS
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
```

Keep in mind that it’s important to add a fallback font. If you’re linking to an external API, you have no guarantee that the URL won’t change, or that the external API won’t go down at some point. Having a reasonable fallback means that if something goes wrong, at least your site won’t look completely broken.

### Text styles: 
#### line height: 

Line height adjusts the space between lines in wrapped text. Adding a little line-height can increase readability
``` css
p.line-height {
  line-height: 1;
}
```
### text-transform
Text transform simply changes the case of the given text. You can use this, for example, to force your heading tags to be all uppercase, or to capitalize every word.
``` css
text-transform: capitalize;
text-transform: uppercase;
text-transform: lowercase;
```

### text shadow :
As you might expect, **text-shadow** adds a shadow around the text in the selected element. This one is best used sparingly, but can be used to great effect in headings or other presentational text.
```css
text-shadow: 1px 1px 2px red, 0 0 1em blue, 0 0 0.2em blue;
```
## Advanced Selectors : 
### Parent and sibling combinators : 

    > - the child combinator
    + - the adjacent sibling combinator
    ~ - the general sibling combinator

We’ll tackle some practical examples using this sample markup.
```html
<main class="parent">
  <div class="child group1">
    <div class="grand-child group1"></div>
  </div>
  <div class="child group2">
    <div class="grand-child group2"></div>
  </div>
  <div class="child group3">
    <div class="grand-child group3"></div>
  </div>
</main>
```


``` css
/* This rule will only select divs with a class of child */
main > div {
  /* Our cool CSS */
}

/* This rule will only select divs with a class of grand-child */
main > div > div {
  /* More cool CSS */
}
```
In order to select an element that is adjacent to our target, or on the same level of indentation, we can use the adjacent sibling combinator +.
``` css
/* This rule will only select the div with the class child group2 */
.group1 + div {
  /* Our cool CSS */
}

/* This rule will only select the div with the class child group3 */
.group1 + div + div {
  /* More cool CSS */
}
```
Finally, if we want to select all of an element’s siblings and not just the first one, we can use the general sibling combinator ~.
``` css
/* This rule will select all of .group1's siblings - in this case the 2nd and 3rd .child divs */
.group1 ~ div {
  /* Our cool CSS */
}
```

### Pseudo Selectors : 
#### **Pseudo Classes :**
  Pseudo-classes offer us different ways to target elements in our HTML. There are quite a lot of them, and they come in a couple of different flavors. Some are based on their position or structure within the HTML. Others are based on the state of a particular element, or how the user is currently interacting with it. There are too many to cover in detail here but we’ll have a look at some of the most useful ones. Pseudo-classes share the same specificity as regular classes (0, 0, 1, 0). Just like regular classes, most can be chained together.

  #### **Structural Pseudo-classes**
**:root** is a special class that represents the very top level of your document - the one element that has no parents. Generally when working with the web, this is equivalent to the html element, but there are a few subtle differences.

:**root** is generally the place where you will place your ‘global’ CSS rules that you want available everywhere - such as your custom properties and CSS variables, or rules such as box-sizing: border-box;

**:first-child** and **:last-child** will match elements that are the first or last sibling.

Similarly **:empty** will match elements that have no children at all, and **:only-child** will match elements that don’t have any siblings.

For a more dynamic approach we can use **:nth-child**. This is a flexible pseudo-class with a few different uses.

#### **Pseudo Elements :**
While pseudo-classes give us an alternative way to interact with our HTML elements based on their state or structure, pseudo-elements are more abstract. They allow us to affect parts of our HTML that aren’t elements at all. These special elements share the same specificity as regular elements (0, 0, 0, 1). There are a number of useful pseudo-elements that can be utilized in any number of creative ways.

**::marker** allows you to customize the styling of your < li > elements’ bullets or numbers.

**::first-letter** and **::first-line** allow you to (you guessed it!) give special styling to the first letter or line of some text.

**::before** and **::after** allow us to add extra elements onto the page with CSS, instead of HTML. Using it to decorate text in various ways is one common use case.

```html
<style>
  .emojify::before {
    content: '😎 🥸 🤓';
}

  .emojify::after {
    content: '🤓 🥸 😎';
}
</style>

<body>
  <div> Let's <span class="emojify">emojify</span>this span!</div>
</body>
```
### Attribute Selectors
Attribute selectors have the same specificity as classes and pseudo-classes (0, 0, 1, 0).

Let’s look at some examples for basic usage.

  * [attribute] - This general selector will select anything where the given attribute exists. Its value doesn’t matter.
  selector
  * [attribute] - Optionally we can combine our attribute selectors with other types of selectors, such as class or element selectors.
  
  * [attribute="value"] - To get really specific, we can use = to match a specific attribute with a specific value
``` css
  [src] {
    /* This will target any element that has a src attribute. */
  }

  img[src] {
    /* This will only target img elements that have a src attribute. */
  }

  img[src="puppy.jpg"] {
    /* This will target img elements with a src attribute that is exactly "puppy.jpg" */
  }
  ```

  ### Positioning : 

  #### **Static and relative postionning :**
  The default positioning mode that you’ve gotten used to is **position: static**. The difference between static and relative is fairly simple. Static is the default position of every element, and properties top, right, bottom, and left do not affect the position of the element. Relative on the other hand is pretty much the same as static, but properties top, ri....(etc.) displace the element relative to its normal position in the flow of the document.


  #### **Absolute postionning :**
**position: absolute** allows you to position something at an exact point on the screen without disturbing the other elements around it. More specifically, using absolute positioning on an element will remove that element from the normal document flow while being positioned relative to an ancestor element. To put it in simple terms: elements that are removed from the normal flow of the document don’t affect other elements and are also not affected by other elements. Using absolute positioning allows you to position elements anywhere on the screen using top, right, bottom, and left properties. This property is really useful when you want to position something at an exact point on the screen, without disturbing any of the other elements

___
## CSS functions : 
### What is a function and how are they used in CSS? :
As in other programming languages, functions are reusable pieces of code which perform specific tasks. Functions are passed “arguments” between parentheses, each of which is used by the function in a specific way. Some common examples are:
``` css 
color: rgb(0, 42, 255);
background: linear-gradient(90deg, blue, red);
```

### **Calc** : 
```css
:root {
--header: 3rem;
--footer: 40px;
--main: calc(100vh - calc(var(--header) + var(--footer)));
}
```
### **min** : 
min() does an excellent job of helping us create responsive websites
```css
#iconHolder {
  width: min(150px, 100%);
  height: min(150px, 100%);
  box-sizing: border-box;
  border: 6px solid blue;
}
```

### **max** : 
``` css
width: max(100px, 4em, 50%);
```
### **clamp**
**clamp()** is a great way to make elements fluid and responsive. **clamp()** takes 3 values:
``` css
h1 {
  font-size: clamp(320px, 80vw, 60rem);
}
```

  * the smallest value (320px)

  * the ideal value (80vw)

 *  the largest value (60rem)

The **clamp()** CSS function uses these values to set the smallest value, ideal value and largest value. In the above example, this would mean the smallest acceptable font-size would be 320px and the largest would be 60rem. The ideal font-size would be 80vw.
