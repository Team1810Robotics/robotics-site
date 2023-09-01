<script>
    import { currentPhoto } from "../store";
    import Link from "$lib/Link.svelte";
    $currentPhoto = "https://www.mvnews.org/wp-content/uploads/2023/04/IMG_6100-900x675.jpg";
</script>

<div class="flex justify-evenly">
    <ul class="flex flex-col gap-6 ml-16 my-6 w-1/2">
        <Link
            mouse="https://www.mvnews.org/wp-content/uploads/2023/04/IMG_6100-900x675.jpg"
            href="https://www.mvnews.org/robotics-team-competes-in-the-greater-kc-regional-competition/"
            text="Robotics team competes in the Greater KC Regional competition"/>
        <Link
            mouse="https://www.mvnews.org/wp-content/uploads/2023/02/CRC_robotics_2-11-133-900x600.jpg"
            href="https://www.mvnews.org/robotics-team-hosts-ftc-competition-saturday-feb-11/"
            text="Robotics team hosts FTC competition Saturday, Feb. 11 "/>
        <Link
            mouse="https://www.mvnews.org/wp-content/uploads/2023/01/photo2-900x600.jpg"
            href="https://www.mvnews.org/senior-isaac-steiner-leads-the-way-for-robotics-and-chess-club/"
            text="Senior Isaac Steiner leads the way for Robotics and Chess Club"/>
        <Link
            mouse="https://www.mvnews.org/wp-content/uploads/2023/01/Screen-Shot-2023-01-10-at-8.23.25-AM-900x423.png"
            href="https://www.mvnews.org/robotics-team-begins-their-season-with-annual-kickoff-event/"
            text="Robotics team begins their season with annual kickoff event"/>
        <Link
            mouse="https://www.mvnews.org/wp-content/uploads/2022/11/IMG_4231-1-900x600.jpg"
            href="https://www.mvnews.org/robotics-competes-at-off-season-competition-cowtown-throwdown-friday-oct-28-and-saturday-oct-29/"
            text="Robotics competes at off-season competition CowTown Throwdown Friday Oct. 28 and Saturday Oct. 29"/>
        <Link
            mouse="https://www.mvnews.org/wp-content/uploads/2022/04/IMG_3605-1-900x600.jpg"
            href="https://www.mvnews.org/robotics-competes-in-the-semi-finals-at-the-central-missouri-regional/"
            text="Gallery: Robotics competes in the semifinals at the Central Missouri Regional"/>
        <Link
            mouse="https://www.mvnews.org/wp-content/uploads/2022/03/26-robotics-147-WEB-900x600.jpg"
            href="https://www.mvnews.org/the-robotics-team-placed-14th-at-the-lees-summit-north-regional-competition/"
            text="The robotics team placed 14th at the Lee's Summit North Regional competition"/>
        <Link
            mouse="https://www.mvnews.org/wp-content/uploads/2022/01/Copy-of-AD_1_8_RoboticsKickoff_IMG_0213-900x600.jpg"
            href="https://www.mvnews.org/first-robotics-competition-begins-season-with-kickoff/"
            text="FIRST Robotics Competition begins season with kickoff"/>
    </ul>
    <img
        src={$currentPhoto}
        alt="First Info"
        class="h-auto max-h-[500px] w-2/6 rounded border-2 border-fg object-cover"/>
</div>