<div id="bg-image"></div>

<style>
    @media (min-aspect-ratio: 1/1) {
        #bg-image {
            background-image: url("/bg/wide.png");
            background-position: center;
            background-size: cover;
            height: calc(100% - 4rem - 2rem);
        }
    }

    @media (max-aspect-ratio: 1/1) {
        #bg-image {
            background-image: url("/bg/tall.png");
            background-position: top;
            background-size: cover;
            height: calc(100% - 4rem - 2rem);
        }
    }
</style>
