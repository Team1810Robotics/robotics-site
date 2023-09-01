<script lang="ts">
    import Link from "$lib/Link.svelte";;
</script>

<div class="flex justify-evenly">
    <ul class="flex flex-col gap-6 ml-16 mt-3 w-fit">
        <Link
            mouse=""
            href="https://www.thebluealliance.com/team/1810"
            text="The Blue Alliance"
            caption="The Blue Alliance is the best way to scout, watch, and relive the FIRST Robotics Competition.<br>You can search by team or event to see history of the team or event."/>
        <Link
            mouse=""
            href="https://www.thebluealliance.com/match/2023mokc_qm26"
            text="FRC Match featuring 1810 CATATRONICS & 9316 CUBATRONICS"
            caption="In the 2023 Greater Kansas City Regional, qualification match twenty-six saw collaboration between two teams: 1810, the varsity team, and 9316, the junior varsity team."/>
    </ul>

    <img
        src="https://www.thebluealliance.com/images/logo_square_512.png"
        alt="Featured"
        class="h-auto w-1/2 mr-16 rounded border-2 border-fg"/>
</div>