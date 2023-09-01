<svelte:head>
    <title>Catatronics | Past Bots</title>
</svelte:head>

<script lang="ts">
    import BackButton from "$lib/BackButton.svelte";
    import Banner from "$lib/Banner.svelte";

    const numberOfImages = 18;
    const images = Array.from({ length: numberOfImages }, (_, i) => numberOfImages - i);
</script>

<BackButton href="/photo"/>
<Banner banner="Past Bots"/>

<ul class="flex flex-wrap justify-center">
    {#each images as i}
        <li class="list-none relative m-0.5 width rounded bg-white">
            <img src="/img/bots/{i}.webp" alt="Past Bot {i}" class="w-full h-auto rounded"/>
        </li>
    {/each}
</ul>

<style lang="postcss">
    .width { width: calc(25% - 5px); }
</style>