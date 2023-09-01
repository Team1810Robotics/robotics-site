<script>
    import { currentPhoto } from "../store";
    import Link from "$lib/Link.svelte";;

    const hoverPhoto = {
        if: "https://www.mvnews.org/wp-content/uploads/2021/03/SC_Robotic_Dog_Bed_6-900x600.jpg",
        gbg: "https://www.mvnews.org/wp-content/uploads/2018/11/IMG_8372EDIT-900x600.jpg"
    }
    $currentPhoto = hoverPhoto.if;
</script>
<div class="flex justify-evenly">
    <ul class="flex flex-col gap-6 ml-16 mt-3 w-fit">
        <Link
            mouse={hoverPhoto.if}
            href="https://www.mvnews.org/robotics-team-creates-and-donates-dog-beds/"
            text="Dog Beds for Imagine Forever Homes"
            caption="Community service project for local charity Imagine Forever Homes, a place for senior dogs to stay until they find their forever home."/>
        <Link
            mouse={hoverPhoto.gbg}
            href="https://www.mvnews.org/robotics-team-modifies-toy-cars-for-special-needs-children/?fbclid=IwAR0eZdF6mD7MX4rIdkALqtEMea7vVX778sUJKZV1VK7ioHHMf1EmyigR6Ro"
            text="Go Baby Go"
            caption="Community Service project with Go Baby Go. Students modify a power wheels vehicle for a special needs child."/>
    </ul>

    <img
        src={$currentPhoto}
        alt="First Info"
        class="h-auto max-h-[500px] w-1/2 rounded border-2 border-fg object-cover"/>
</div>