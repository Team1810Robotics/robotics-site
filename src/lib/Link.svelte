<script lang="ts">
    import { currentPhoto } from "../routes/link-articles/store";

    export let href: string;
    export let text: string;
    export let caption: null | string = null;
    export let mouse: string;
</script>

<li class="text-w text-xl rounded-lg px-4 group" on:mouseenter={() => $currentPhoto = mouse }>
    <a href={href} target="_blank">{text}</a>
    <span class="block max-w-0 group-hover:max-w-full transition-all duration-300 h-px bg-w max-lg:hidden"></span>
    {#if caption}
        <span class="text-sm ml-4 font-thin">{@html caption}</span>
    {/if}
</li>