<script lang="ts">
	import Feed from './Feed.svelte';

	let events = [1, 2, 3];
</script>

<Feed items={events} let:item>
	<div>{item}</div>

	<footer slot="footer">Footer</footer>
</Feed>
