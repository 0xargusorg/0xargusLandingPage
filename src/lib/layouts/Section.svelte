<script lang="ts">
	import { cn } from '$lib/utils/cn';
	export let className = $$props.class || '';
	export let maxWidth = '7xl';
	export let id = '';
</script>

<section
	{id}
	class={cn(`flex w-full items-center justify-center px-4 py-8 sm:px-12 sm:py-16 ${className}`)}>
	<div class={cn(`max-w-${maxWidth} grid w-full`)}>
		<slot />
	</div>

	<slot name="background" />
</section>
