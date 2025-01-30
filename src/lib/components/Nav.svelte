<script lang="ts">
    import NavLink from './NavLink.svelte';
    import { ScrollArea } from './ui/scroll-area';
    import * as Sheet from './ui/sheet';
    import { Icon } from 'svelte-icons-pack';
    import { BiMenuAltLeft } from 'svelte-icons-pack/bi';

    let open = $state(false);
</script>

<Sheet.Root bind:open>
    <Sheet.Trigger class="absolute left-4">
        <Icon src={BiMenuAltLeft} color="white" size="24" />
    </Sheet.Trigger>
    <Sheet.Content side="left">
        <NavLink href="/" bind:open class="text-cyan-200">Lightning Creations</NavLink>
        <ScrollArea orientation="both" class="my-4">
            <div class="flex flex-col space-y-3">
                <NavLink href="/about" bind:open>About</NavLink>
                <NavLink href="/contact" bind:open>Contact</NavLink>
            </div>
            <div class="flex flex-col space-y-2 pt-6">
                <h4 class="text-lg">Outside Links</h4>
                <NavLink href="https://discord.gg/mkBtTMk6cA" bind:open>Discord</NavLink>
                <NavLink href="https://github.com/LightningCreations" bind:open>GitHub</NavLink>
            </div>
            <p class="pt-6 text-slate-400">More to come, watch this space...</p>
        </ScrollArea>
    </Sheet.Content>
</Sheet.Root>
