<script>
	let count = 0;

	function increase() {
		count++;
	}

	let array = [ 1, 2, 3, 4 ];
	
	function addItem() {
		array.push( array.length + 1 );
		console.log( array );
	}
</script>

<main>
	<h1>Simple Counter</h1>

	<p>Count : { count }</p>

	<button on:click={ increase }>Add count</button>

	<p>List : { JSON.stringify( array ) }</p>

	<button on:click={ addItem }>Add Item to List</button>
</main>
