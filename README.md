# challenge-sass

## The basic concepts of Sass:

 Sass is a programming/scripting language. I bet you didn't see that one coming. Yes, it's a programming/scripting language focused on increasing the efficiency of web designers and web developers creating CSS.


---


 ### The following concepts 


 - Sass or SCSS
- Variables
- Mixins
- Arguments
- Nesting
- Partial files
- @import
- Source maps
- Sass comments

---

### Sass or SCSS
There are two ways we can write Sass-style CSS: the Sass syntax and the SCSS syntax.

#### *Tip*
Make no mistake; Sass is written with capital S and the rest with lower case and SCSS is all uppercase.


----------

### The Sass syntax
The Sass syntax, also known as the indented syntax, was the initial and only way to write Sass. But it looked a bit too different than regular CSS, making the learning curve steeper than it really needed to be.

---
###  basic example:


     .selector-a
          float: left
 
        .selector-b
            background: orange
            
           

## about Sass mixins are as follows:

-         They start with the @mixin directive
 -         A mixin is called with the @include directive
  -        We can store any amount of CSS/SCSS data in a mixin
   -       Try to use arguments when creating a mixin so it's more calable

## mixin examples 

    $brandBlue: #416e8e;
    $supportGray: #ccc;
    @mixin genericContainer {
        padding: 10px;
        border: $brandBlue 1px solid;
        background: $supportGray;
         box-shadow: 1px 1px 1px rgba(black, .3);
     }


### In mixin call a as selector in scss file 

     .selector-a {
          @include genericContainer;
     }


 #### When compiled, it looks like this in the CSS:
         .selector-a {
    padding: 10px;
    border: #416e8e 1px solid;
    background: #cccccc;
    box-shadow: 1px 1px 1px rgba(0, 0, 0, 0.3);
     }


[Github Repo](https://github.com/galalkoro/challenge-sass)