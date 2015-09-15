# SASS
http://sass-lang.com/install
#
#### INSTALACIÓN WINDOWS
1) instalar ruby ->http://rubyinstaller.org/
#
2) $ gem install sass
#
3) $ sudo gem install sass

#
#### RUN
sass --watch estilos.scss:estilos.css
#

#### MIXIN
```sass
//*--- 	Mixin Fonts ---*
@mixin fonts($font)
	@font-face
		font-family: $font
		src: url('../fonts/#{$font}.eot')
		src: url('../fonts/#{$font}.eot?#iefix') format('embedded-opentype'),
		url('../fonts/#{$font}.woff') format('woff'), 
		url('../fonts/#{$font}.ttf') format('truetype'), 
		url('../fonts/#{$font}.svg#$font') format('svg')

@include fonts('Forza-Book')
@include fonts('Forza-Black') 
@include fonts('Forza-Bold') 

```
