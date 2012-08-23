#glyphicons.less
A less file to ease the use of the [GLYPHICONS](http://glyphicons.com/).

###Usage
In your LESS-file setup and import glyphicons.less

```less
@import "../glyphicons";

 .icon {
	@url: "../glyphicons-free/glyphicons-halflings.png";
	@url-white: "../glyphicons-free/glyphicons-halflings-white.png";
	@icon-width: 14px;
	@icon-height: 14px;

	// Generate base css
	#glyphicons > .layout(@url, @icon-width, @icon-height);

	// Add white theme css
	&.white {
		#glyphicons > .theme(@url-white);
	}

	&.icon-glass {#glyphicons > .icon(0, 0);}
}
```

*For more details see examples*


Adding icons is simple just add this wherever you want an icon. The code below will give you the icon named `glass`.

```css
<i class="icon icon-glass"></i>
```

###About GLYPHICONS
GLYPHICONS is a library of precisely prepared monochromatic icons and symbols,
created with an emphasis on simplicity and easy orientation.
More info about the icons here: [GLYPHICONS.com](http://glyphicons.com/)