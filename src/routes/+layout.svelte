<script lang="ts">
    import Nav from '$lib/components/Nav.svelte';
    import '../app.css';
    let { children } = $props();
</script>

<div class="h-screen flex flex-col">
    <div class="flex h-16 flex-row items-center justify-center bg-muted">
        <Nav />
        <h1 class="text-3xl"><a href="/">Lightning Creations</a></h1>
    </div>
    <div class="overflow-scroll flex-1">
        {@render children()}
    </div>
    <div class="flex h-8 items-center justify-center bg-muted">
        <p class="text-xs">&copy; 2025 Lightning Creations</p>
    </div>
</div>
