<script lang="ts">
    import type { HTMLAnchorAttributes } from "svelte/elements";

	let {
		href,
		...restProps
	}: HTMLAnchorAttributes = $props();
</script>

<a class="text-cyan-100 underline" href={"mailto:" + href}>{href}</a>