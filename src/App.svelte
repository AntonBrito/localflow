<script>
	import ReviewList from "./components/ReviewList.svelte"


	let review = [
		{
			id: 1,
			rating: 10,
			text: 'Lorem ipsum dolor sir amet consecteur adipisicing elit.consecteur vel avitae commodi alias voluptartem est voluptatum ipsa quae.',
		},
		{
			id: 2,
			rating: 7,
			text: 'Lorem ipsum dolor sir amet consecteur adipisicing elit.consecteur vel avitae commodi alias voluptartem est voluptatum ipsa quae.',
		},{
			id: 3,
			rating: 5,
			text: 'Lorem ipsum dolor sir amet consecteur adipisicing elit.consecteur vel avitae commodi alias voluptartem est voluptatum ipsa quae.',
		}
	]

</script>

<main class="container">
	<ReviewList {review}/>
</main>

<style>
	
</style>