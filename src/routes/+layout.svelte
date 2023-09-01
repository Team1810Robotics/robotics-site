<script lang="ts">
    import "../app.css";

    const links = [
        /* {
            name: "Home",
            href: "/",
            target: "_self",
        }, */
        {
            name: "Calendar",
            href: "https://www.usd232.org/Page/5145",
            target: "_blank",
        },
        {
            name: "Photo Gallery",
            href: "/photos",
            target: "_self",
        },
        {
            name: "Sponsors",
            href: "/sponsors",
            target: "_self",
        },
        {
            name: "Regional Info",
            href: "/regional-info",
            target: "_self",
        },
        {
            name: "Links & Articles",
            href: "/link-articles",
            target: "_self",
        },
        {
            name: "Forms",
            href: "/forms",
            target: "_self",
        },
    ];


</script>

<nav class="flex justify-evenly items-center bg-fg text-w font-bold h-[8vh]">
    <a href="/" class="uppercase letterspace-wide text-xl group">
        Catatronics
        <span class="block max-w-0 group-hover:max-w-full transition-all duration-300 h-0.5 bg-w max-lg:hidden"></span>
    </a>
    <ul class="nav-links letterspace-thin font-thin relative text-sm hidden justify-around w-4/5 lg:flex">
        {#each links as link}
            <li class="group">
                <a href={link.href} target={link.target}>{link.name}</a>
                <span class="block max-w-0 group-hover:max-w-full transition-all duration-300 h-px bg-w max-lg:hidden"></span>
            </li>
        {/each}
    </ul>
</nav>

<slot/>

<style lang="postcss">
    .letterspace-wide {
        letter-spacing: 5px;
    }
    .letterspace-thin {
        letter-spacing: 2px;
    }
</style>