<script lang="ts">
import Inc from "./inc.svelte";

	export let name: string;
</script>

<main>
	<Inc/>

</main>
<style global lang="postcss">
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
</style>
