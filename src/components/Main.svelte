<script>
    import Step from "./Step.svelte";

    let steps = [
        { name: "Northcoders News", icon: "fa-solid fa-newspaper" },
        { name: "Game Master", icon: "fa-solid fa-dice" },
        { name: "Workout App", icon: "fa-solid fa-dumbbell" },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center text-center lg:text=left gap-6 md:gap-8 lg:gap-10"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi I'm <span class="poppins text-violet-400">Jamie</span> Lewis
                <br />Full Stack
                <span class="poppins text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-violet-400">favourite tech</span> includes JavaScript
                (NEXT.JS or SvelteKit), TailwindCSS, Node.js + Express.js & PostgreSQL
                or Firebase/Firestore!
            </p>
            <a
                href="https://www.linkedin.com/in/jamie-lewis-42b376b4"
                target="_blank"
                class="blueShadow mx-auto lg:mr-auto text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <!-- <img
                src={"images/profile.png"}
                alt="Profile Image"
                class="object-cover z-[2] max-h-[70vh]"
            /> -->
        </div>
    </section>
    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-lg sm:text-xl md:text-2xl">
                A few of my creative endeavours.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-violet-400">see</span> my work?
            </h3>
        </div>
        <a
            href=""
            target="_blank"
            class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
        >
            <i class="fa-regular fa-circle-play" />
            <p>Watch the video</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>
                    Northcoders news is a social news platform created as part
                    of my Northcoders bootcamp using <strong
                        class="text-violet-400"
                        >ReactJS, Node.js, Express.js + PostgreSQL!</strong
                    >It allows for users to post articles, and like and comment
                    other peoples articles.
                </p>
            </Step>
            <Step step={steps[1]}>
                <p>
                    Game Master is a <strong class="text-violet-400"
                        >React Native, Node.js, Express.js, MongoDB, Firebase
                        and socket.io</strong
                    > app which was created as part of a project team during the
                    Northcoders bootcamp. It allows a user to create and search for
                    gaming events. It includes a chat feature, and a levelling system
                    as a reward for attending or hosting events.
                </p>
            </Step>

            <Step step={steps[2]}>
                <p>
                    FitTracker is a fitness excersizes app built using<strong
                        class="text-violet-400"
                        >React, Node.js, MaterialUI, RapidAPI</strong
                    >
                </p>
            </Step>
        </div>
    </section>
    <section id="about">Hey</section>
</main>
