# CSS Associates Style rules with HTML elements

*CSS works by associating rules with HTML elements. These rules govern 
how the content of specified elements should be displayed. A CSS rule 
contains two parts: a selector and a declaration.*

**CSS declarations sit inside curly brackets and each is made up of two 
parts: a property and a value, separated by a colon.**

### using External CSS
-  **<link>**
the link element can be used 
in an HTML document to tell the 
browser where to find the CSS 
file used to style the page.

- ** href**
This specifies the path to the 
CSS file (which is often placed in 
a folder called css or styles).
- ** type**
This attribute specifies the type 
of document being linked to. The 
value should be text/css

- **rel**
This specifies the relationship between the HTML page and the file it is linked to. The value should be stylesheet when linking to a CSS file .

### Using Internal CSS

**<style>**
You can also include CSS rules within an HTML page placing them inside a style element, which usually sits inside the head element of the page. The style element should use the type attribute to indicate that the styles are specified in CSS. The value should be text/css.

### CSS Selectors
![selector](https://i.pinimg.com/originals/46/ca/fc/46cafc70b7bdd146745e2e600c06019d.png)

** CSS rules usually appear in a separate document, 
although they may appear within an HTML page.**

## color
*The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways*
1.rgb values
2.hex codes
3.color names

### background-color
CSS treats each HTML element as if it appears in a box, and the background-color property sets the color of the background for that box.

**Every color on a computer screen is created by mixing amounts of red, green, and blue. To find the color you want, you can use a color picker.**

![color](https://cdn5.vectorstock.com/i/1000x1000/41/24/rgb-color-mode-wheel-mixing-vector-16834124.jpg)

### HSL Colors
CSS3 introduces an entirely new and intuitive 
way to specify colors using hue, saturation, 
and lightness values.

- **hue**
Hue is the colloquial idea of 
color. In HSL colors, hue is often 
represented as a color circle 
where the angle represents the 
color, although it may also be 
shown as a slider with values 
from 0 to 360.

 - **saturation**
Saturation is the amount of 
gray in a color. Saturation is 
represented as a percentage. 
100% is full saturation and 0% 
is a shade of gray.

- **lightness**
Lightness is the amount of 
white (lightness) or black 
(darkness) in a color. Lightness 
is represented as a percentage. 
0% lightness is black, 100% 
lightness is white, and 50% 
lightness is normal. Lightness 
is sometimes referred to as 
luminosity

** CSS3 also allows you to specify colors as HSL values, 
with an optional opacity value. It is known as HSLA**



