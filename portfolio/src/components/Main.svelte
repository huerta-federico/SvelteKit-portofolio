<script>
    import Step from "./Step.svelte";

    let steps = [
        {name: "Project 1", icon: "fa-brands fa-linux", description:""},
        {name: "Project 2", icon: "", description: ""},
        {name: "Project 3", icon: "", description: ""},
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
        >
            <!-- Section title -->
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins text-violet-400">Federico</span>
                Huerta
                <br />IT Engineering
                <span class="poppins text-violet-400">Student</span>
            </h2>

            <!-- Section subtitle -->
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-violet-400"> favorite stuff</span> includes
                things, cookies, more stuff, bits and pieces, and you guessed it,
                EVEN MOAR STUFF!
            </p>

            <!-- Get in Touch button-->
            <a
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
                href="a"
                target="_blank"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </a>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/profile.png"}
                alt="Zetane Engine"
                class="object-cover z-[2] max-h-[70vh]"
            />
        </div>
    </section>
    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:textxl">A few of my stuff</h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-violet-400">see</span> my stuff?
            </h3>
        </div>
        <a
            href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
            target="_blank"
            class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
        >
            <i class="fa-regular fa-circle-play" />
            <p>Watch the video</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>Project 1 is just a placeholder for the description of stuff, things and stuff.</p>
            </Step>
            <Step step={steps[1]}></Step>
            <Step step={steps[2]}></Step>
        </div>

    </section>
</main>
