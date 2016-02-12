# SELECTORS

	- What are the selectors ?
	- Selecting Nodes by Tag names
	-	Selecting Nodes by ID
	- Selecting Nodes by Class Name
	- Selecting Nodes by Attribute value
	- Selecting Input Nodes
	- Additional Selector Features

## What are the selectors ?

	- Selectors allow page elements to be selected.
	- Single or multiple elements are supported.
	- A selector identifies an HTML element/tag that you will you manipulate with jQuery.

	 For Example:

	<div id="freshersDiv" class="freshersClass">
		<span class="welcomeClass"> Welcome Learners </span>
	</div>

## selector Syntax

			$(selectorExpression)
			jQuery(selectorExpression)

## Selecting Nodes by Tag names

	- $('p') - select all <p> elements.
	- $('a') - select all <a> elements.

	## To reference multiple tags, use the , character to separate the elements:

	$('p,a,span') - select all paragraphs anchors and span elements.

## Selecting Descendants

		- $('ancestor descendant') selects all descendants of the ancestor.

					$('table tr')
		* Here selects all tr elements that are descendants of the table element.
		* Descendants are  children,grandchildren,etc of the designated ancestor element.
