# Responsive Design Course notes

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
## CSS : 