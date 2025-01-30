<script lang="ts">
    import type { HTMLAnchorAttributes } from "svelte/elements";

	let {
		open = $bindable(false),
		href,
		children,
		...restProps
	}: HTMLAnchorAttributes & { open: boolean } = $props();

	function handleClick() {
		open = false;
	}
</script>

<a
	{href}
	onclick={handleClick}
	{...restProps}
>
	{@render children?.()}
</a>