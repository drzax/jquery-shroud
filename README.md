This jQuery plugin drops a shroud over any element on a page, and that's about it.

There are, I will freely admit, many a jQuery plugin to achieve exactly what 
this plugin does. At some point I searched and wasn't happy with what I found
so I built this for my own use.

== Usage ==
```
$('.selector').shroud([command][, options]);
```

If the <code>command</code> parameter is omitted, the <code>'drop'</code> command
is assumed (see below).

The following commands are supported:
```
'drop'		// Drops the shroud over the selected elements.
'lift'		// Lifts the shroud from the selected elements.
'destroy'	// Lifts the shroud from the selected elements and removes it entirely from the DOM.
```

The following options are available:
```
// Default options exposed so they can be updated globally.
$.fn.shroud.defaults = {
	opacity: .8,			// Opacity of the shroud
	z: 100,					// z-index for the shroud element
	color: '#000',			// Shroud color
	speed: 200,				// Effect speed
	click: false,			// If set to true, the shroud will be removed when clicked
	destroy: false,			// Completely remove shroud from DOM after lifting? (only applies when lift function is called)
	complete: null			// A callback to execute on completion of drop or lift.
}
```

== Feedback, Bug Reports & Contributions ===
Support requests and bug reports can be posted to the 
GitHub issue tracker](https://github.com/drzax/jquery-shroud/issues). If you'd 
like to help improve jQuery.shroud feel free to submit a pull request via GitHub.

<a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/"><img alt="Creative Commons License" style="border-width:0" src="http://i.creativecommons.org/l/by-sa/3.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/3.0/">Creative Commons Attribution-ShareAlike 3.0 Unported License</a>.


