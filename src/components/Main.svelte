<script>
    import Step from "./Step.svelte";

    let steps = [
        {
            id:1,
            name: "Pulzion",
            icon: "fa-solid fa-p",
            href:"https://pulzion.co.in",
            description:
                "Pulzion is the annual flagship event organized by PICT ACM Student Chapter (PASC). Pulzion consists of multiple events in technical as well as non-technical domains including coding competitions, mock placement interviews, business management-based events, design and development based contests and quizzing events.",
        },
        {
            id:2,
            name: "Movie-Land",
            icon: "fa-solid fa-clapperboard",
            href:'https://movieland-7000.netlify.app/',
            description:
                "Based on the OMDB API.",
        },
        {
            id:3,
            name: "PASC Alumni Portal(Upcoming)",
            icon: "fa-solid fa-diagram-project",
            description:
                "Built for the students of PICT ACM Student Chapter to get in touch with their alumni, so that students can benefit from the Alumni network",
        },
    ];

    let benefits = [
        {
            metric: "10x",
            name: "A Student at P.I.C.T",
            description:
                "I am a pre final year student at the Pune Institute of Computer Technology (P.I.C.T), I am pursuing my B.E. in Computer Engineering.",
        },
        {
            name: "Web Development Enthusiast",
            description:
                "I am interested in learning new technologies in the domain of web development. And I am constantly learning and improving my skills, building new projects.",
        },
        {
            name: "An excellent communicator",
            description:
                "Communication is key and it's a paramount value of mine. I believe in transparency and constructive communication above all else. This helps me develop deep relationships and ensures my effectiveness and productivity in any work space with any team.",
        },
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
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="lucida text-violet-400">Aditya</span> More
                <br />Full Stack
                <span class="lucida text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-violet-400"> favorite tech</span> includes JavaScript
                (NEXT.JS or SvelteKit),TypeScript, TailwindCSS, Node.js + Express.js & MongoDB!
            </p>
            <button
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl lucida relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <a href="https://www.linkedin.com/in/aditya-more-9a095422a/" target="_blank">
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </a>
            </button>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/profile.jpg"}
                alt="Zetane Engine"
                class="object-cover z-[2] max-h-[70vh] rounded-full"
            />
        </div>
    </section>
    <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                A few of my creative endeavors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="lucida text-violet-400">see</span> my work?
            </h3>
        </div>
        <a
            href="https://www.linkedin.com/posts/pict-acm-student-chapter-09004a132_big-props-to-the-pasc-web-team-for-putting-activity-7121522688442953728-Q7Kx?utm_source=share&utm_medium=member_desktop"
            target="_blank"
            class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
        >
            <i class="fa-regular fa-circle-play" />
            <p>Watch the video</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>
                    <strong
                    class="text-violet-400"
                    >Built using The PERN Stack!</strong
                >
                    Pulzion is the annual flagship event organized by PICT ACM Student Chapter (PASC). Pulzion consists of multiple events in technical as well as non-technical domains including coding competitions, mock placement interviews, business management-based events, design and development based contests and quizzing events.

                </p>
            </Step>
            <Step step={steps[1]}>
                <p>
                    Movie-Land is a front end <strong
                        class="text-violet-400">React.js</strong
                    > application
                    that allows a user to search for movies, it makes use of the <strong class="text-violet-400">OMDB API</strong>
                </p>
            </Step>
            <Step step={steps[2]}>
                <p>
                    PASC Alumni Portal a <strong class="text-violet-400"
                        >PERN Stack</strong
                    >
                    web application, that is built for the students of PICT ACM Student Chapter to get in touch with their alumni, so that students can benefit from the <strong class="text-violet-400">Alumni network</strong>
                </p>
            </Step>
        </div>
    </section>
    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <!-- <div class="z-[-1] bg-violet-950 w-screen left-1/2 -translate-x-1/2 top-0 h-full absolute"> </div> -->
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
        >
            <h6 class="text-large sm:text-xl md:text-2xl">
                Want to know more?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="lucida text-violet-400">about</span> me.
            </h3>
        </div>
        <p class="mx-auto lucida font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <div class="flex gap-6 sm:gap-8">
                    <p
                        class="lucida text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
                    >
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            {benefit.name}
                        </h3>
                        <p>{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>
        <h5 class={" text-2xl sm:text-3xl font-semibold text-center lucida "}>
            The <span class="text-violet-400">Complete</span> Package
        </h5>
        <div
            class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full"
        >
            <table class="bg-white text-slate-700 rounded text-center">
                <thead class={"border-b border-solid border-slate-200  "}>
                    <tr class="">
                        <th />
                        <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                        <th
                            class="bg-violet-700 text-white whitespace-nowrap p-4 px-8"
                            >Me</th
                        >
                    </tr>
                </thead>
                <tbody>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Dedication</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Critical Thought</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr>
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Interpersonal Skills</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-t border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Progamming Ability</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                </tbody>
            </table>
        </div>
        <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
            <p>Scroll to see more &rarr;</p>
        </div>
        <p class="mx-auto">So why not invest?</p>
    </section>
</main>