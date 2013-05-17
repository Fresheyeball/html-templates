html-templates
==============

Html templates won the hard way with FIRE! Released and maintained here as Open Source.

# Usage

These templates are generated with [jade](http://jade-lang.com/) which is a most excellent templating language and markup preprocessor. There is no need to use the jade versions at all. If you like you can simple edit the html files found in `/html` to suit your needs. 

However should you choose to use the jade files you will need either 
 - [node.js](http://nodejs.org/) with the [jade npm](https://npmjs.org/package/jade) installed
 - [codekit](http://incident57.com/codekit/) a stand alone OSX application that processes any front end language you wish

You can then take advantage of the `mixin`s found in `/jade/mixins`, which will allow you to quickly and easily custom generate an html template.

## Mixins

All arguments are optional. Depending on your version of jade, arguments may need to be all on one line :(

	```coffeescript
	mixin metaItems({
		allowIE8 	: <boolean>,
		html5shive	: <path to html5 (defaults to cdn)>
		author 		: <string>,
		title 		: <string>,
		description : <string>,
		designer 	: <string>,
		copyright 	: <string copyright holder's name>
	})

	mixin mobile({
		apple 		: <path to apple icon directory>,
		viewport 	: <viewport meta content>
	})

	mixin googleAnalytics({
		code : <Google Analytics ID>,
		egar : <BOOLEAN optional>
	})	

	mixin facebook({
		title 		: <title for facebook>,
		description : <html description for facebook>,
		image 		: <path to image>
	})	
	```

# Purpose

These templates are intended to be the minimum necessary recommended for as many usecases as possible. That means as little opinion as possible, which means no 'twitter bootstrap', 'jquery', 'knockout' or any other libraries. Also, no Paul Irish conditional comments or other hacks are included.

Adding any of those components to the template assumes asset pipeline along with about 50 other things about how the template is to be used. If you want jQuery from the CDN add it, its cool, its about what you want. :)



