<svelte:head>
    <title>Catatronics | Sponsors</title>
</svelte:head>

<script lang="ts">
    import Banner from "$lib/Banner.svelte";
import { images } from "./sponsors";
</script>

<Banner banner="Sponsors"/>

<!-- NOTE: Images expect to be a 1:1 aspect ratio -->
<div class="flex flex-wrap justify-center mb-5">
    {#each images as i}
        <a class="list-none relative m-0.5 width rounded bg-white" href={i.href} target="_blank">
            <img src={i.src} alt={i.alt} class="w-full h-auto rounded"/>
        </a>
    {/each}
</div>

<style lang="postcss">
    .width { width: calc(33% - 10px); }
</style>