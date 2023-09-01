<svelte:head>
    <title>Catatronics | Home</title>
</svelte:head>

<div class="overflow-hidden h-[85vh]">
    <div class="bg-home bg-fixed bg-center bg-no-repeat bg-cover h-full w-full blur"></div>
</div>

<div class="container text-w font-bold backdrop-blur-3xl border-2 border-w bg-[#00000099] p-5">
    <h1 class="text-center text-[2.5rem]">Hello, This is FRC Team<br>1810 & 9316</h1>
    <hr class="mt-4">
    <!-- <h2 class="text-center text-base border-b border-w pb-4"></h2> -->
</div>

<div class="text-w bg-fg px-12 pb-12">
    <h1 class="text-center text-3xl font-bold p-8">About Us:</h1>
    <div class="flex flex-wrap justify-center gap-3 mb-8">
        <p class="w-5/6">
            &emsp;FIRST (For Inspiration and Recognition of Science and Technology) Robotics Teams 1810 & 9316, aka 1810 Catatronics and 9316 Cubatronics, is comprised of students from both the DeSoto and Mill Valley high schools in USD232.
            The students work together to build a robot that solves the challenges presented by FIRST Robotics in each year's game, thereby expanding our knowledge of STEM principles.
            Our team is comprised of students that focus on CAD & design, manufacturing, electrical, programming, scouting & strategy, and business sub-teams.
            Students are encouraged to try all the sub-teams.
            We strive to work cohesively as a team, ensuring that each student is able to take these experiences into their future career paths.
        </p>
        <p class="w-5/6">
            Teams design, build, and program industrial-sized robots to play a difficult field game against like-minded competitors.
            We have six weeks to accomplish that goal.
            Our focus is to promote STEM in our school and community and is achieved through outreach projects, fundraising, and presentations.
        </p>
    </div>
    <hr class="mt-4">

    <!-- <h3 class="text-center text-3xl font-bold">Check Out:</h3>
    <ul class="list-disc list-outside text-xl leading-10">
        <li>The <a class="italic text-link hover:underline visited:text-link-visited" href="https://www.usd232.org/Domain/3832" target=_blank> District Page</a> For The Teams</li>
        <li>The <a class="italic text-link hover:underline visited:text-link-visited" href="https://github.com/Team1810Robotics" target=_blank>Github</a> That Holds Our Code</li>
        <hr class="mt-4">
    </ul> -->



    <h3 class="text-center text-2xl font-bold">Contact Us:</h3>
    <div class="text-xl leading-10 flex justify-evenly">
        <div>
            Neil McLeod
            <ul class="list-disc ml-12">
                <li>nmcleod@usd232.org</li>
                <li>(913) 422-4351 ext 3140</li>
            </ul>
        </div>
        <div>
            Dianna Worm Mayfield
            <ul class="list-disc ml-12">
                <li>dworm@usd232.org</li>
                <li>(913) 620-2920</li>
            </ul>
        </div>
    </div>
</div>

<style lang="postcss">

    :global(body) {
        background-color: #0d1117;
    }

    .container {
        /* TODO: use better way to center */
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);

        width: clamp(300px, 40%, 700px);
        box-shadow: 10px 10px 10px 5px rgba(0, 0, 32, 0.2);
    }
</style>