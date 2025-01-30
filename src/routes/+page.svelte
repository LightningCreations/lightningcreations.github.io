<svelte:head>
    <title>Lightning Creations</title>
</svelte:head>

<div id="bg-image" class="h-full"></div>

<style>
    @media (min-aspect-ratio: 1/1) {
        #bg-image {
            background-image: url("/bg/wide.png");
            background-position: center;
            background-size: cover;
        }
    }

    @media (max-aspect-ratio: 1/1) {
        #bg-image {
            background-image: url("/bg/tall.png");
            background-position: top;
            background-size: cover;
        }
    }
</style>
