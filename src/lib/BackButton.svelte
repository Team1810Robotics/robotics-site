<script lang="ts">
    export let href: string;
</script>

<a class="back flex justify-center rounded bg-fg text-w p-2 w-24 transition-all duration-500 cursor-pointer m-1 ml-2 shadow-md group" href={href}>
    <span class="cursor-pointer inline-block relative duration-500 group-hover:pl-6 after:absolute after:opacity-0 after:top-0 after:-left-5 after:duration-500 after:content-['\00ab'] group-hover:after:opacity-100 group-hover:after:left-0">
        Back
    </span>
</a>