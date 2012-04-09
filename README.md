# jQuery Stylewords

For the times when you wish that CSS had a :first-word(x) psuedo-class.

## Getting Started
Download the [production version][min] or the [development version][max].

[min]: https://raw.github.com/jeffreyway/jquery.styleWords/master/dist/jquery.styleWords.min.js
[max]: https://raw.github.com/jeffreyway/jquery.styleWords/master/dist/jquery.styleWords.js

In your web page:

```html
<p>Lorem ipsum dolor sit amet.</p>
<script src="jquery.js"></script>
<script src="dist/jquery.styleWords.min.js"></script>
<script>
jQuery(function($) {
  $('p').styleWords(2);
});
</script>
```

This will turn the paragraph into:

```html
<p><span class="styleWords">Lorem ipsum</span> dolor sit amet.</p>
```

At this point, you have your CSS hook. Style those first few words however you wish!

## Examples

### Easiest Usage

	// Filter through collection, and wrap the 
	// first word in a span.
	$('p').styleWords();


	// Wrap the first three words in a span
	$('p').styleWords(3);


	// Wrap the first two words, and use a `strong` tag instead.
	$('p').styleWords(2, {
		tag: '<strong>'
	});


	// Apply a custom classname
	$('p').styleWords(2, {
		'class': 'my-custom-class'
	});

## Release History
- 0.1.0 - First draft of plugin.

## License
Copyright (c) 2012 Jeffrey Way  
Licensed under the GPL license.
