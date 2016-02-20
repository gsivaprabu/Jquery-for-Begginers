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
## Selectings node by ID
	- In Javascript we using document.getElementByID.
	- use the # character used to select the particular id.
	- $('#myIdName')

## Selecting Nodes by Class Name
	- Use the . character to select elements by class name
	- $(.myClassName)
	- selects <p class="myClassName"> element
	- Use multiple class names use , to separate the class
	- $('.blueDiv,.redDiv')
	- $(a.myClassName) - select only <a> tags with myClassName
## Selecting Nodes by Attribute value
	-Use brackets[attribute] to select based on attribute name and/or attribute value:
		-$('a[title]')  Select all <a> elements that have a title attribute
		- $('a[title="Programming Info"]')
			- Select all programing elements that have a "Programming Info" title attribute value.

## Selecting Input Nodes
	-$(':input') select all input elements including: input,select,textarea,button,image,radio and more
	 $(':input[type="radio"]')
	- targrt all radio buttons on the page.. but it is the most efficent selector.

## Additional Selector Features
	- Selectors based on specific tag name.
	- using contains in selector
	- :contains() will select elements that match the contents with the contains exception.

			$('div:contains("sivaprabu")')

	- select the div's that contain the text sivaprabu (note that the match in case sensitive)
	- <div> I love javascript by sivaprabu </div>

	- Selecting Even or Odd rows in a table
	- $('tr:odd') and$('tr:even') is the jQuerysyntax for selecting odd or even rows respectively.
	- Remember the index is 0 based - the first two row in the table is 0:
		- Odd will return [1,3,5,7,9]..etc
		- Even will return [0,2,4,6,8]..etc

		-	Selecting the First Child
			-$('element:first-child') select the first child of every element group.
			-$('span:first-child')

									<div>
										<span>First Child, First Group</span>
										<span>Second Child, First Group</span>
									</div>
									<div>
										<span>First Child</span>
										<span>Second Child, Second Group Child </span>
									</div>
	- Using start with in selectors

	- [attribute^="value"] will select all elements with an attribute that  begins with stated value.
	- [attribute*="value"] will select all elements with an attribute that  an attribute with stated value.

	- $('input[value^="Events"]')
	- select any input element whose value attribute begins with "Events":

		<input type="button"value="Events - World"/>
		<input type="button"value="Events - National"/>
		<input type="button"value="Events - Local"/>

	- Find attributes containing a value
		[attribute*="value"] will select all elements with an attribute that contain the stated value:

			$('input[value*="Events"]')

			select any input element whose value attribute contains "Events":

				<input type="button" value="World Events 2011">
				<input type="button" value="National Events 2011">
				<input type="button" value="Local Events 2011">