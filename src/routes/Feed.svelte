<script lang="ts">
	export let items: any[];
</script>

<!-- 500 happens when we iterate over items and pass item as a slot prop-->
<!--  && there is another named slot -->
<!-- HACKY FIX 1: only use named slots -->
{#each items as item}
	<slot {item} />
{/each}

<!-- HACKY FIX 2: only have one slot -->
<slot name="footer" />
