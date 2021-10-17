<script>
  export let review = []
  console.log(review)
</script>

{#each review as rv (rv.id)}
  <h3>{rv.text}</h3>
{/each}