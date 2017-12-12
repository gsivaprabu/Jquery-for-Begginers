# INTERACTING WITH DOM ELEMENTS

	-	How can interact with Document Object Model
			- Iterating through Nodes.
			- Modifying DOM object properties.
			- Modifying Attributes
			- Adding and removing Nodes.
			- Modifying Styles.
			- Modifying Classes.

# ITERATING THROUGH NODES
### each()
	.each(function(index,Element)) is used to iterate through jQuery objects.

		$('div').each(function(index){
					alert(index+'='+$(this).text());
			})
### this is raw DOM Object

	iterates through each div element and returns its index number and text

		$('div').each(function(index,elem){
				alert(index+'='+$(elem).text());
			})
### elem = this values are same

# MODIFYING PROPERTIES AND ATTRIBUTES
	- jQuery easy to interact with DOM element.
	- Modifying object properties
		- The this.propertyName statement can be used to modify an object's propertiesdirectly:
				$('div').each(function(i){
						this.title="My Index = "+i;
					});
	- Iterates through each div and modifies the title. If the property does not exist, it will be added.
	- this represenet the raw DOM Object.
### Object attributes can be accessed using attr():
	- var val = $('#divId').attr('title'); here retrieves the value of the title attribute.
### Modifying Attributes
	- .attr(attributeName,value) is the method used to access an object's attributes and modify the value:
		$('img').attr('title','My Image title');
	- Changes the title attribute to a value of My Image Title.
### Modifying multiple attributes
	- To modify multiple attributes,pass a JSON object containing name /value pairs.
			$('img').attr({
					title:'My Image Title',
					style:'border:2px solid black'
				})
	- JSON objec tpassed and used to change title and border.
