<script>
	import ReviewList from "./components/ReviewList.svelte";
	import Nav from './components/Nav.svelte';


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
		},
		{
			id: 3,
			rating: 5,
			text: 'Lorem ipsum dolor sir amet consecteur adipisicing elit.consecteur vel avitae commodi alias voluptartem est voluptatum ipsa quae.',
		}
	]

	const deleteReview = (e) => {
		const itemId = e.detail
		review = review.filter((item) => item.id != itemId)
	}

</script>
<Nav />
<main class="container">
	<ReviewList {review} on:delete-review={deleteReview} />
</main>

