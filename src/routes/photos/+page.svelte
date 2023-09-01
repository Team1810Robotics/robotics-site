<svelte:head>
    <title>Catatronics | Photos</title>
</svelte:head>

<script lang="ts">

    const buttons = [
        {
            href: "gallery/past-bots",
            // Image aspect ratio [24 / 29]
            img: "/img/bots/old-bots.webp",
            name: "Past Bots",
        },
        {
            href: "gallery/season/2022S",
            img: "/img/seasons/2022S/2022s.webp",
            name: "2022 Season",
        },
        {
            href: "gallery/season/2021S",
            // Image aspect ratio [24 / 29]
            img: "/img/seasons/2021S/2021s.webp",
            name: "2021 Season",
        },
        {
            href: "gallery/season/2020S",
            // Image aspect ratio [24 / 29]
            img: "/img/seasons/2020S/2020s.webp",
            name: "2020 Season",
        },
        {
            href: "gallery/season/2019S",
            // Image aspect ratio [24 / 29]
            img: "/img/seasons/2019S/2019s.webp",
            name: "2019 Season",
        },
        {
            href: "gallery/season/2018S",
            // Image aspect ratio [24 / 29]
            img: "/img/seasons/2018S/2018s.webp",
            name: "2018 Season",
        },
        {
            href: "gallery/season/2017S",
            // Image aspect ratio [24 / 29]
            img: "/img/seasons/2017S/2017s.webp",
            name: "2017 Season",
        },
        {
            href: "gallery/season/2016S",
            // Image aspect ratio [24 / 29]
            img: "/img/seasons/2016S/2016s.webp",
            name: "2016 Season",
        },
        {
            href: "gallery/season/2015S",
            // Image aspect ratio [24 / 29]
            img: "/img/seasons/2015S/2015s.webp",
            name: "2015 Season",
        },
        /* {
            // "3" photos but 2 are the same photo
            href: "gallery/season/2014S",
            // Image aspect ratio [24 / 29]
            img: "/img/seasons/2014S/2014s.webp",
            name: "2014 Season",
        }, */
        {
            href: "gallery/season/2013S",
            // Image aspect ratio [24 / 29]
            img: "/img/seasons/2013S/2013s.webp",
            name: "2013 Season",
        },
        {
            href: "gallery/season/2012S",
            // Image aspect ratio [24 / 29]
            img: "/img/seasons/2012S/2012s.webp",
            name: "2012 Season",
        },
        {
            href: "gallery/season/2011S",
            // Image aspect ratio [24 / 29]
            img: "/img/seasons/2011S/2011s.webp",
            name: "2011 Season",
        },
        {
            href: "gallery/season/2010S",
            // Image aspect ratio [24 / 29]
            img: "/img/seasons/2010S/2010s.webp",
            name: "2010 Season",
        },
        {
            href: "gallery/season/2009S",
            // Image aspect ratio [24 / 29]
            img: "/img/seasons/2009S/2009s.webp",
            name: "2009 Season",
        },
        {
            href: "gallery/season/2008S",
            // Image aspect ratio [24 / 29]
            img: "/img/seasons/2008S/2008s.webp",
            name: "2008 Season",
        },
        {
            href: "gallery/season/2007S",
            // Image aspect ratio [24 / 29]
            img: "/img/seasons/2007S/2007s.webp",
            name: "2007 Season",
        },
        {
            href: "gallery/season/2006S",
            // Image aspect ratio [24 / 29]
            img: "/img/seasons/2006S/2006s.webp",
            name: "2006 Season",
        }
    ];
</script>

<div class="mt-3 flex flex-row flex-wrap justify-evenly gap-2 will-change-transform transition-transform duration-500">
    {#each buttons as btn}
        <div class="bg-fg flex flex-col rounded-md auto-width h-auto text-center deep-shadow group
            hover:transition-all hover:ease duration-300 hover:transform hover:-translate-y-1">
            <a href={btn.href}>
                <img
                class="w-full h-auto border-2 border-fg rounded-md"
                src={btn.img}
                alt={btn.name}/>
            </a>
            <a href={btn.href} class="text-w text-2xl m-2 p-2 group-hover:underline">{btn.name}</a>
        </div>
    {/each}
</div>

<style lang="postcss">
    .auto-width {
        width: calc(25% - 50px);
    }

    .deep-shadow {
        box-shadow: 5px 5px 4px 1px rgba(0,0,0, 0.2);
    }

    .deep-shadow:hover {
        box-shadow: 10px 10px 8px 2px rgba(0,0,0, 0.2);
    }
</style>