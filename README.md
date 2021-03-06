# Sequence-action - v1.0.1
===

Use to animate all childrens of a given element in sequence, simply select items one by one, and toggle class "on".

## Params

	animateSequence(_target, _params);
	
* **_target**, *String* (Required) : Parent of the items to animates (ul, div, etc) 
* **_params**, *Array* (Optional) :  
	* **direction**, *string* : 
		* **forward**: Animate from first to last child (default)
		* **backward**: Animate from last to first child
	* **duration**, *int* : Time in **ms** between each step (default : **100ms**)
	* **callback**, *function* : Do what you whant


## Use

Load **animate-sequence.js** in your page.

Simply call the animate-sequence function

	animateSequence(_target, _params);

You can only animate adjacent children of a given parent.

For example all **li** of a list:

	Js:
	
	animateSequence('ul', {
		direction: 'backward',
		duration: 100,
		callback: function(){
			//Anything you want;
		}
	});
	
	Html:
	
	<ul>
		<li>Item 1</li>
		<li>Item 2</li>
		<li>Item 3</li>
		<li>Item 4</li>
		<li>Item 5</li>
		<li>Item 6</li>
	</ul>
	
Or any childs of a given parent. They don't need to be similar tag.

	<article>
		<p>Items 1</p>
		<div>Items 2</div>
		<img src="" alt="Items 3" />
		...
	</article>

You can check into /demo (or live at [lab.crucifixarnaud.com/js/sequence-action](http://lab.crucifixarnaud.com/js/sequence-action) for an example using css transition on a list.

## Support


Browsers allready tested:

* **Firefox 3.6+**
* **Chrome 8+**
* **Safari v5.1+**
* **Opera 11.5+**
* **Internet Explorer 10+**

* **Safari Mobile**
* **Android (v4+) Android Browser**
* **Android (v4+) Chrome**



## Changelog

* **v1.0** Initial Release
	* *v1.0.0*: _params, direction (forward, backward), duration, callback
	* *v1.0.1*: Update doc, sequence-action.min.js


## Credits

Created by Crucifix Arnaud ([crucifixarnaud.com](http://crucifixarnaud.com))

This is free and unencumbered software released into the public domain. ([http://unlicense.org]())
