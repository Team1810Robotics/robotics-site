<svelte:head>
    <title>Catatronics | Links & Articles</title>
</svelte:head>

<script lang="ts">
    import Banner from "$lib/Banner.svelte";
    import FirstInfo from "./components/FirstInfo.svelte";
    import Interest from "./components/Interest.svelte";
    import Outreach from "./components/Outreach.svelte";
    import TbaInfo from "./components/TBAInfo.svelte";

    enum Pages {
        FIRSTInfo,
        TBAInfo,
        Outreach,
        Interest
    }

    let page: Pages = Pages.FIRSTInfo;
</script>

<Banner banner="Robotics Links & Sites"/>

<div class="flex justify-evenly text-w text-lg font-thin m-4">
    <button class={`p-4 w-1/6 rounded-lg hover:bg-blue-950 transition duration-300 ${(page === Pages.FIRSTInfo)  ? "bg-blue-900 italic" : "bg-fg" }`} on:click={() => page = Pages.FIRSTInfo}>FIRST Info</button>
    <button class={`p-4 w-1/6 rounded-lg hover:bg-blue-950 transition duration-300 ${(page === Pages.TBAInfo)    ? "bg-blue-900 italic" : "bg-fg" }`} on:click={() => page = Pages.TBAInfo}>Blue Alliance Info</button>
    <button class={`p-4 w-1/6 rounded-lg hover:bg-blue-950 transition duration-300 ${(page === Pages.Outreach)   ? "bg-blue-900 italic" : "bg-fg" }`} on:click={() => page = Pages.Outreach}>Robotics Outreach</button>
    <button class={`p-4 w-1/6 rounded-lg hover:bg-blue-950 transition duration-300 ${(page === Pages.Interest)   ? "bg-blue-900 italic" : "bg-fg" }`} on:click={() => page = Pages.Interest}>Links of Intrest</button>
    <!-- <a class="p-4 w-1/6 rounded-lg text-center hover:bg-blue-950 bg-fg transition duration-300" href="https://drive.google.com/drive/folders/1XN_UjbLO_zUWwdwXBCuGdan9jDdr8G8A?usp=sharing" target="_blank">CAD Files</a> -->
</div>

{#if page === Pages.FIRSTInfo}
    <FirstInfo/>
{:else if page === Pages.TBAInfo}
    <TbaInfo/>
{:else if page === Pages.Outreach}
    <Outreach/>
{:else if page === Pages.Interest}
    <Interest/>
{/if}