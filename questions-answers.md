#Questions

###1.The `input` element has an attribute called "type." Discuss the purpose and function of this attribute, and list some of the values 'type' can be.

The HTML <input> tag is used within a form to declare an input element - a control that allows the user to input data. With the `type` attribute, you tell it what type of input you want it to be. If you want a input of a simple button just write `type="button"` or if you want a email, date, image, telephone number and more.

###2.Describe what a "next-sibling selector" is. Explain how it works and give an example of its usage.

The next-sibling selector (+) lets you select an elements immediately sibling.

HTML:
```html
<p>Hello there!</p>
<p>How are you today?</p><!--Immediate sibling of the first <p>-->
```

CSS:
```css
p + p {/*you select the sibling by putting "+" in between the two p's*/
	background-color: blue;
}
```

###3.The C in CSS stands for "Cascade". What does this terminology mean and what is its significance to how CSS is interpreted?

CSS or Cascading Style Sheets is where you put make up on your web page or style it the way you want it to look. All you need is to select a element from your HTML and add the style. Lets say you want to select all p tags and change the color of the font:
```css
p {
	color: red;
}
```
This is all you do to style it. Now, what if later you select the p element and put a different color? Which one would CSS pick? Easy, CSS would pick the last selector. That's why it's called "Cascading" Style Sheets, CSS checks your selectors from top to bottom and applies your styles.

###4.Explain in detail what the CSS Box Model is.

####Title: The CSS Box Model
Category: The Box Model

The CSS box model is exactly what its name is, a box. You can think of HTML elements as boxes. All HTML elements are wrapped in a box. It consist of **margins, borders, padding and the content**. 

Here is a example of the box model:

![box model](http://www.codeproject.com/KB/HTML/567385/boxmodel-image.png)

Lets start with the margin of the box model. The *margin* is transparent and gives it space outside the border. The *border* surrounds the padding and content. The *padding* is like the margin but instead of being outside the border, it's inside the border. The content is where the text and images will appear.

For every element in HTML, you can change its width and height of the box model. In other words, you change the width and height of the margin, border and padding. This is a example for changing the box model:

```css
section {
    width: 350px;
    padding: 20px;
    border: 3px dash red;
    margin: 0; 
}
```

Even dou width is set to 350px, it is not 350px. You have to include the padding, border and margin.

`350(width)+40(left+right padding)+6(left+right border)+0(left+right margin) = 396px = width`


###5.Explain how the `border` property and its variants `border-top`, `border-right`, `border-bottom`, and `border-left` works. Be sure to point out the values that this property takes and the effects those values can have on the display of elements.

The border property helps you decorate or outline the border of your CSS box model. You can customise each side with different styles or widths. The `border-top`, `border-right`, `border-bottom`, and `border-left` lets you choose individually or you can just use `border` and add the different values. The different values include: width, style like solid or dotted line, color of the line and more.

border-top: 5px;
border-right: 7px;
border-bottom: 5px
border-left: 7px;

is the same as...

border: 5px 7px 5px 7px;
or
border: 5px 7px;










