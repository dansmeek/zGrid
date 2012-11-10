zGrid
---
zGrid is a light-weight, responsive, flexible, grid with lots of options.

I developed zGrid to offer a grid system to encompass features from other responsive design grids... all were good, but a certain element was always missing.   I also wanted it be lightweight, and customizable. Larger browsers show too much white space for 960px based grids.    

I wanted to incorporate nesting, various breakpoints, convenient spacing, and modification.

I wanted the math to be done entirely by the compiler. So you only have to worry about specifying what you want. Such as your max-width, breakpoints, number-of-columns, fluid layout, etc.


-----------------

This project is still in development and -- as such -- is not 100% tested. If you are using the CSS file then this should work fine.

-----------------------
Usage
---
Forkit or cloneit. Make any changes you would like to the sass file and then simply type:

sass zgrid.scss [filename]

the naming conventions in the sass file are relatively straightforward. I would not recommend changing the full width percent to less than 90%.

Examples
---
~~~~~~~~~~~~~~~~~~~~~~~~~~
row = new row

c1 through c(n) creates a column of size (n), size being dependant on how many columns you have specified.

a row within a column will create a column of size n/2.

a1 through a(n) sets the "alpha" spacing of the column.  
- This is static.   a(n) will have the same properties regardless of which column its applied to.

o0 through o(16) sets the "omega" spacing.   
- using o0 will specify a column to be aligned to the right most side.
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

 - e.g class = "c5 o0" --> fixes a column of size5 to the right margin

 - "a3 c4" --> specified a column of size4 to be pushed 3 alpha units right.

 - "a2 c2 end" --> specifies a column to be pushed 2 alpha units left from the previous column and specifies that it is also the last column in the row

 - More uses, demo: http://www.wontstop.net/demos/zgrid/

 - If you only intend to use the CSS file, it was compiled using a 16 column layout with standard tablet and smartphone breakpoints. With a responsive design and a full width of 1200px.
