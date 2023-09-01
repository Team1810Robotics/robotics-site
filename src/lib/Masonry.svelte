<script lang="ts">
    export let images: number[];
    export let hightClass: string;
    export let src: string;
    export let alt: string;
</script>

<div class="flex flex-col flex-wrap content-between w-[97%] gallery gap-1 {hightClass}">
    {#each images as i}
        <div class="w-1/3 m-0 ml-1 relative gallery-image">
            <img
            src={`${src}-${i}.webp`}
            alt={alt}
            class="w-full h-auto rounded-md bg-fg text-w"/>
        </div>
    {/each}
</div>

<style lang="postcss">
    /* Re-order items */
    .gallery-image:nth-child(3n+1) { order: 1; }
    .gallery-image:nth-child(3n+2) { order: 2; }
    .gallery-image:nth-child(3n)   { order: 3; }

    /* Force new columns */
    .gallery::before,
    .gallery::after {
        content: "";
        flex-basis: 100%;
        width: 0;
        order: 2;
    }
</style>