<script lang="ts">
    import '../app.css';
    let { children } = $props();
</script>

<div class="h-screen bg-zinc-900">
    <div class="flex h-16 flex-row items-center justify-center bg-zinc-800">
        <h1 class="font-lc text-3xl text-white">Lightning Creations</h1>
    </div>
    {@render children()}
    <div class="flex h-8 items-center justify-center">
        <p class="text-xs text-white">&copy; 2025 Lightning Creations</p>
    </div>
</div>
