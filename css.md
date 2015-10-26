# css

#### Centrar vertical
http://www.fontsquirrel.com/tools/webfont-generator
#
http://www.font2web.com/

```html
<style type="text/css">
    div.parent {
         position: relative;
    }

    /*vertical middle and horizontal center align*/
    img.child {
        bottom: 0;
        left: 0;
        margin: auto;
        position: absolute;
        right: 0;
        top: 0;
    }
    </style>

    <div class="parent">
        <img class="child"> 
    </div>
```

#### FontFace
http://www.fontsquirrel.com/tools/webfont-generator
#
http://www.font2web.com/

```css

@font-face {
    font-family: 'brandon_grotesque_regularRg';
    src: url('brandon_reg-webfont.eot');
    src: url('brandon_reg-webfont.eot?#iefix') format('embedded-opentype'),
         url('brandon_reg-webfont.woff2') format('woff2'),
         url('brandon_reg-webfont.woff') format('woff'),
         url('brandon_reg-webfont.ttf') format('truetype'),
         url('brandon_reg-webfont.svg#brandon_grotesque_regularRg') format('svg');
    font-weight: normal;
    font-style: normal;

}
```
#
#### Generador de sombras
http://www.css3maker.com/box-shadow.html


#### Personalizar checkbox

```html
<form class="blockCheckbox">
    <input type="radio" name="option" id="radio1"  />
    <label for="radio1">Hombre</label><br />
    <input type="radio" name="option" id="radio2" />
    <label for="radio2">Mujer</label><br />
    <input type="checkbox" name="option" id="check1"  />
    <label for="check1">DVD</label><br />
    <input type="checkbox" name="option" id="check2" />
    <label for="check2">CD</label>
  </form>
```

```css

.blockCheckbox

	input[type="radio"], input[type="checkbox"]
		display: none

	label
		padding-left: 1.25em
		background: url('front/img/check.png') no-repeat 
		background-size: 16px 16px

	input[type="radio"] + label
		width: 16px
		height: 16px

	input[type="radio"]:checked + label
		background: url('front/img/checked.png') no-repeat 
		width: 16px
		height: 16px
		background-size: 16px 16px

	input[type="checkbox"] + label
		width: 16px 
		height: 16px
		

	input[type="checkbox"]:checked + label
		background: url('front/img/checked.png') no-repeat 
		width: 16px
		height: 16px
		background-size: 16px 16px
```
#



