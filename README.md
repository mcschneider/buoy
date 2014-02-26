# Buoy
Buoy is a simple micro-library that makes working with vanilla JS a little bit easier, by [Chris Ferdinandi](http://gomakethings.com).

* Add, remove, toggle and check for classes.
* Get an object's sibling elements.

[View the Demo](http://cferdinandi.github.io/buoy/)

1. [Getting Started](#getting-started)
2. [Browser Compatability](#browser-compatability)
3. [Options & Settings](#options-and-settings)
4. [Changelog](#changelog)
5. [License](#license)



## Getting Started

### 1. Include Buoy on your site.

	<script src="js/buoy.js"></script>

### 2. Use Buoy in your scripts.

`hasClass( element, class )` - Check if an element has a class.

	var turkey = document.querySelector('#turkey');
	if ( buoy.hasClass(turkey, 'sandwich') ) {
	    // Do stuff...
	}

`addClass( element, class )` - Add a class to an element.

	var turkey = document.querySelector('#turkey');
	buoy.addClass(turkey, 'sandwich');

`removeClass( element, class )` - Remove a class from an element.

	var turkey = document.querySelector('#turkey');
	buoy.removeClass(turkey, 'sandwich');

`toggleClass( element, class )` - Add or remove a class from an element.

	var turkey = document.querySelector('#turkey');
	buoy.toggleClass(turkey, 'sandwich');

`getSiblings( element )` - Get an array of siblings for an element.

	var turkey = document.querySelector('#turkey');
	var turkeyFriends = buoy.getSiblings(turkey);
	Array.prototype.forEach.call(turkeyFriends, function (friends) {
	    // Do stuff...
	});

And that's it, you're done. Nice work! New to vanilla JS? Check out [Ditching jQuery for Vanilla JS](http://gomakethings.com/ditching-jquery-for-vanilla-js/).



## Brower Compatability

Buoy works in all modern browsers, and IE 6 and above.



## Changelog
* v1.2 (November 10, 2013)
  * Updated regex patterns.
  * Added `classList` function for supporting browsers.
  * Both updates adapted from [Apollo by Todd Motto](https://github.com/toddmotto/apollo).
* v1.1 (August 27, 2013)
  * Added missing semicolons.
  * Activated strict mode.
* v1.0 (August 26, 2013)
  * Initial release.



## License
Buoy is licensed under the [MIT License](http://gomakethings.com/mit/).