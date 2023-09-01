<script lang="ts">
    import type { PageData } from "./$types";
    import { numberOfPhotos } from "$lib";
    import BackButton from "$lib/BackButton.svelte";
    import Masonry from "$lib/Masonry.svelte";
    import Banner from "$lib/Banner.svelte";
    import "$lib/heights.css";

    export let data: PageData; 
    const slug = data.slug;
    const year = slug.slice(0, 4);

    var num = numberOfPhotos.get(slug);
    const images = Array.from({length: (num ?? 0)}, (_, i) => (num ?? 0) - i);
</script>

<svelte:head>
    <title>Catatronics | {year} Season</title>
</svelte:head>

<BackButton href="/photos"/>

<Banner banner="{year} Season"/>

<Masonry images={images} hightClass="s{year}" src={`/img/seasons/${slug}/${slug.toLowerCase()}`} alt="{year} Season"/>