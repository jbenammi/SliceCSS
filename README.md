SliceCSS
(v1.0.0)
This is an open-source css framework build off of fundamentals started by Bootstrap, Materialize and W3CSS.
The basis for this new framework is to create a more granular RWD grid based on a 16 grid system and utilizing only CSS and Javascript.


##### INSTALATION #####

To use SliceCSS, place the SCSS(SASS) or CSS file in your program folder containing all the cascading style sheets you will use.
You should then be able to use all the tag and class functionality as described below.

``` CSS
<link rel="stylesheet" type="text/css" href="./../path/to/your/folder/slice.css">
<link rel="stylesheet" type="text/css" href="./../path/to/your/folder/slice.scss">

```

Some items may utilize javascript depending on how you want to deploy the element.

To use SliceCSS js, you can either place the js code directly into your html document or point to the slice.js file.

``` JS
<style type="text/css">
		var modal = function(id1, id2){
			document.getElementById(id1).style.display='block';
			document.getElementById(id2).style.float='none';
		}
		var modalClose = function(id1){
			document.getElementById(id1).style.display='none';
		}
</style>
```

``` JS
<style type="text/css" src="./../path/to/your/folder/slice.js"></style>
```


##### DOCUMENTATION #####
Please Note:
This is a very rough start to this framework. As it is built out better documentation will be updated for easier use.

1: Initialization
2: Type-Face

//// forthcoming documentation ////
3: Height/Width/Justification
4: RWD Grid
5: Colors
6: Elements
	6-1: Navigation Bar/Links
	6-2: Modal
	6-3: Buttons
	6-4: Forms


##### 1: Initialization #####

This normalizes the CSS for your project so that you are working with a clean code base. It removes some of the presets set up by the different browsers as it renders your code.
At the moment it has very minimal normalization for padding, margin, box-sizing and webkit margins. 


##### 2: Type-Face #####

The main font being used in SliceCSS is Cicle. The files are included in the install but can also be found at the following site. (https://www.fontsquirrel.com/fonts/Cicle).

To use, make sure the @font-face in the slice.css file points to the installation folder location. This will need to be done for;
cicleFina
cicleGordita
cicleShadow

``` CSS
@font-face {
    font-family: 'cicleFina';
    src: url('../font/cicle_fina_macroman/Cicle_Fina-webfont.eot');
    src: url('../font/cicle_fina_macroman/Cicle_Fina-webfont.eot?#iefix') format('embedded-opentype'),
         url('../font/cicle_fina_macroman/Cicle_Fina-webfont.woff') format('woff'),
         url('../font/cicle_fina_macroman/Cicle_Fina-webfont.ttf') format('truetype'),
         url('../font/cicle_fina_macroman/Cicle_Fina-webfont.svg#ciclefina') format('svg');
    font-weight: normal;
    font-style: normal;
}
```


##### CONTRIBUTIONS #####

If you are interested contributing to the project you can fork the project from;
https://github.com/jbenammi/SliceCSS.git. 
Consideration will be given to all contributions if they are CSS/JS dependent only. Any contributions with JQuery or other library dependencies will not be considered for this project as it runs counter to the project reasoning.

##### License #####

The MIT License (MIT)

Copyright (c) 2016 Jonathan Ben-Ammi

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.