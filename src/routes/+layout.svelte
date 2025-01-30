<script lang="ts">
    import Nav from '$lib/components/Nav.svelte';
    import '../app.css';
    let { children } = $props();
</script>

<svelte:head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous">
    <link href="https://fonts.googleapis.com/css2?family=Atkinson+Hyperlegible:ital,wght@0,400;0,700;1,400;1,700&display=swap" rel="stylesheet">
</svelte:head>

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
