# Sequence-action - v1.0
===

Use to animate all childrens of a given element in sequence, simply select items one by one, and toggle class "on".

## Use

Load **animate-sequence.js** in your page.

Simply call the animate-sequence function

	animateSequence(_target, _params);
	
* **_target** (Required) : Parent of the items to animates (ul, div, etc) 
* **_params** (Optional) :  
	* **_direction** : 
		* **forward**: Animate from first to last child (default)
		* **backward**: Animate from last to first child
	* **_duration**: Time in **ms** between each step (default : **60ms**)
	* **_callback**: Do what you whant

You can only animate adjacent children of a given parent.

For example all **li** of a list:

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

You can check [demo.html]() for an example using css transition on a list.

## Support


Browsers allready tested:

* **Firefox 3.6+**
* **Chrome**
* **Safari (v5?)**
* **Opera (v10?)**

* **Safari Mobile**
* **Android (v4+) Android Browser**
* **Android (v4+) Chrome**

Not currently test:

* **ie10**
* **ie9**
* **ie8**
* **ie7**



## Changelog

* **v1.0** Initial Release
	* _params : direction (forward, backward), duration, callback


## Credits

Created by Crucifix Arnaud ([crucifixarnaud.com]())

This is free and unencumbered software released into the public domain. ([unlicense.org]())
