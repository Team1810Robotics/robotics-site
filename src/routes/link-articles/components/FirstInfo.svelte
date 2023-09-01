<script>
    import { currentPhoto } from "../store";
    import Link from "$lib/Link.svelte";;

    const hoverPhoto = {
        teaser: "https://info.firstinspires.org/hs-fs/hubfs/first_in_show/ChangedUp_2022_Feature_Image_1.webp?width=2000&name=ChangedUp_2022_Feature_Image_1.webp",
        vision: "https://www.firstinspires.org/sites/default/files/uploads/about/leadership/dean-kid-headshot-vm.png",
        about: "https://www.firstinspires.org/sites/all/themes/first/assets/images/2020/program-block-frc.jpg",
        vr: "https://7002112.fs1.hubspotusercontent-na1.net/hubfs/7002112/first-vr-campaign/vr/stats-img.jpg",
        kc: "https://www.kcfirst.org/wp-content/uploads/2014/07/FIRST_Robotics_KC_Regional_Saturday_3_14_2015-3562_opt.jpg",
    };
    $currentPhoto = hoverPhoto.teaser;
</script>

<div class="flex justify-evenly">
    <ul class="flex flex-col gap-6 ml-16 mt-3 w-fit">
        <Link
            mouse={hoverPhoto.teaser}
            href="https://info.firstinspires.org/first-in-show"
            text="Teaser Video for FIRST 2024 FRC Theme"/>
        <Link
            mouse={hoverPhoto.vision}
            href="https://www.firstinspires.org/about/vision-and-mission"
            text="FIRST Vision & Mission"/>
        <Link
            mouse={hoverPhoto.about}
            href="https://www.firstinspires.org/"
            text="Learn more about FIRST"
            caption="For Inspiration and Recognition of Science and Technology"/>
        <Link
            mouse={hoverPhoto.vr}
            href="https://info.firstinspires.org/vr?utm_source=email&utm_medium=mc&utm_campaign=vr-experience&_hsenc=p2ANqtz--OUrI4oAfdiTEwYiSn85a3eMKPx87taDDaCc6VPhqdYbBM5zghf5g9aNeiaIGASbYVqFAL5c6pGlk9Edp8vY8oDQhoZQ&_hsmi=93686148&hsCtaTracking=e0502955-6eb1-4d12-823c-523"
            text="FIRST Robotics VR experience"/>
        <Link
            mouse={hoverPhoto.kc}
            href="https://www.kcfirst.org/"
            text="KC FIRST Information"
            caption="Information about FIRST Robotics in Kansas City Metro"/>
    </ul>

    <img
        src={$currentPhoto}
        alt="First Info"
        class="h-auto max-h-[500px] w-1/2 rounded border-2 border-fg object-cover"/>
</div>