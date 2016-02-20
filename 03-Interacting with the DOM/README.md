# INTERACTING WITH DOM ELEMENTS

	-	How can interact with Document Object Model
			- Iterating through Nodes.
			- Modifying DOM object properties.
			- Modifying Attributes
			- Adding and removing Nodes.
			- Modifying Styles.
			- Modifying Classes.

# ITERATING THROUGH NODES
## each()
	.each(function(index,Element)) is used to iterate through jQuery objects.

		$('div').each(function(index){
					alert(index+'='+$(this).text());
			})
### this is raw DOM Object

	iterates through each div element and returns its index number and text

		$('div').each(function(index,elem){
				alert(index+'='+$(elem).text());
			})
### elem = this


