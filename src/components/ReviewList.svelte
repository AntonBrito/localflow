<script>
  import ReviewItem from "./ReviewItem.svelte";
  export let review = []
  
</script>

{#each review as rv (rv.id)}
  <ReviewItem item={rv} />
{/each}