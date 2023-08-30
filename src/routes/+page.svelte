<script>
    let bioItems = [
        { name: "Discord personal assistant", description: "", icon: "" },
        {
            name: "Interact with our interdimensional goddess via SQL based commands",
            description: "",
            icon: "",
        },
        {
            name: "Start now with no strings attached",
            description: "",
            icon: "",
        },
    ];

    let steps = [
        {
            name: "Organization & Planning",
            icon: "fa-solid fa-calendar-days",
            description:
                "Interact with Jasmine via a set of SQL inspired commands to manage your organization and planning. Jasmine will remind you of upcoming events, keep a record of your todos, and much much more.",
        },
        {
            name: "Data & Analytics",
            icon: "fa-solid fa-chart-pie",
            description:
                "Test for model robustness with customized test profiles and receive exhaustive reporting on the performance and potential vulnerabilities of your model.",
        },
        {
            name: "No Apps or Downloads",
            icon: "fa-solid fa-check-double",
            description:
                "Augment your datasets with our filters and dataset manipulations to ensure your models are trained on the highest quality datasets (coming soon).",
        },
    ];

    let benefits = [
        {
            metric: "10x",
            name: "join the Discord channel",
            description:
                "Conduct rigorous automated testing and auditing with Zetane Protector to ensure your AI solution is robust and trustable. Zetane Protector is a cloud-based tool that was engineered to significantly reduce the development cycle time required to bring AI projects to operational readiness with more confidence.",
        },
        {
            name: "open a private chat window with Jasmine",
            description:
                "Explain and diagnose machine learning models with the Zetane Insight Engine to eliminate black box limitations, gain deep actionable insights and quickly improve and validate your AI models.",
        },
        {
            name: "type /start to begin",
            description:
                "Using our suite of software and proven expertise, Zetane can help you make your models more robust, accurate and adapted to your operational context.",
        },
    ];
</script>

<main class="mx-auto max-w-[1200px] w-full p-4 sm:p-6">
    <section
        id="mainPage"
        class="min-h-screen flex flex-col gap-4 sm:gap-6 md:gap-8"
    >
        <div class=" mt-6 sm:mt-12 md:mt-16 py-4 text-white mr-auto ">
            <h1 class="text-6xl sm:text-7xl md:text-8xl font-semibold">
                Try <span class="poppins text-emerald-400">Jasmine</span>
            </h1>
        </div>
        <div
            class="flex flex-col gap-10 sm:gap-12 md:gap-16 border-l-8 border-solid border-emerald-400 pt-6 sm:pt-10 md:pt-14 ml-4 sm:ml-6 md:ml-8"
        >
            {#each bioItems as item}
                <div class="flex flex-col gap-4">
                    <div class="flex items-center gap-4">
                        <div
                            class="w-10 sm:w-16 md:w-24 h-2 shrink-0 bg-emerald-400"
                        />
                        <h3
                            class="text-2xl sm:text-3xl md:text-4xl lg:text-5xl font-extralight"
                        >
                            {item.name}
                        </h3>
                    </div>
                </div>
            {/each}
        </div>
        <div class="mx-auto pt-10">
            <button
                class="flex relative after:absolute after:bg-white after:bottom-0 after:right-full after:h-[1.5px] after:w-full hover:after:translate-x-full after:duration-200 overflow-hidden"
            >
                <p class="poppins z-10">
                    Start <span class="poppins text-emerald-400">chatting</span>
                    today &rarr;
                </p>
            </button>
        </div>
    </section>
    <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-lg sm:text-xl md:text-2xl font-light">
                The goddess of organization.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                How does <span class="poppins text-emerald-400">she</span> work?
            </h3>
        </div>
        <a
            href="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
            target="_blank"
            class="mx-auto px-4 py-2 rounded-full border border-solid border-emerald-950 flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-emerald-600 duration-200"
        >
            <p>Watch the video</p>
            <i class="fa-regular fa-circle-play" />
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <div
                target="_blank"
                class="p-4 sm:p-6 md:p-8 flex flex-col gap-4 rounded-lg border border-solid border-emerald-950 text-center cursor-pointer group hover:border-emerald-600 duration-200"
            >
                <div
                    class="bg-slate-950 grid place-items-center px-4 text-5xl md:text-6xl -mt-10 sm:-mt-12 md:-mt-14 lg:-mt-16 mx-auto duration-200"
                >
                    <i class={steps[0].icon} />
                </div>
                <h3 class="font-medium text-xl sm:text-2xl md:text-3xl">
                    {steps[0].name}
                </h3>
                <div class="flex flex-1 flex-col justify-center items-center">
                    <p>
                        Interact with Jasmine via a set of <strong
                            class="text-emerald-400">SQL based commands</strong
                        >
                        to manage and optimize your organization and planning. Jasmine
                        is the ultimate
                        <strong class="text-emerald-400"
                            >personal assistant.</strong
                        >
                    </p>
                </div>
                <a
                    href="#"
                    target="_blank"
                    class=" font-light mx-auto relative after:absolute after:h-full after:w-full after:top-0 after:right-full after:bg-emerald-500 after:duration-200 hover:after:translate-x-full after:z-[-1] overflow-hidden"
                >
                    Get started &rarr;
                </a>
            </div>
            <div
                target="_blank"
                class="p-4 sm:p-6 md:p-8 flex flex-col gap-4 rounded-lg border border-solid border-emerald-950 text-center cursor-pointer group hover:border-emerald-600 duration-200"
            >
                <div
                    class="bg-slate-950 grid place-items-center px-4 text-5xl md:text-6xl -mt-10 sm:-mt-12 md:-mt-14 lg:-mt-16 mx-auto duration-200"
                >
                    <i class={steps[1].icon} />
                </div>
                <h3 class="font-medium text-xl sm:text-2xl md:text-3xl">
                    {steps[1].name}
                </h3>
                <div class="flex flex-1 flex-col justify-center items-center">
                    <p class="">
                        Jasmine has a <strong class="text-emerald-400"
                            >fetch function</strong
                        >
                        which allows Jasmine to retrieve from your own API's. Furthermore,
                        Jasmine can create
                        <strong class="text-emerald-400"
                            >daily summaries of tasks and analytics</strong
                        > as you please.
                    </p>
                </div>
                <p class=" font-light">Coming soon!</p>
            </div>
            <div
                target="_blank"
                class="p-4 sm:p-6 md:p-8 flex flex-col gap-4 rounded-lg border border-solid border-emerald-950 text-center cursor-pointer group hover:border-emerald-600 duration-200"
            >
                <div
                    class="bg-slate-950 grid place-items-center px-4 text-5xl md:text-6xl -mt-10 sm:-mt-12 md:-mt-14 lg:-mt-16 mx-auto duration-200"
                >
                    <i class={steps[2].icon} />
                </div>
                <h3 class="font-medium text-xl sm:text-2xl md:text-3xl">
                    {steps[2].name}
                </h3>
                <div class="flex flex-1 flex-col justify-center items-center">
                    <p>
                        You can access Jasmine on any device <strong
                            class="text-emerald-400">without</strong
                        >
                        the need to any
                        <strong class="text-emerald-400"
                            >downloads or apps</strong
                        >. Organize your plans in a simple Discord chat window - all you
                        need is a
                        <strong class="text-emerald-400">Discord account</strong
                        >.
                    </p>
                </div>
                <a
                    href="#"
                    target="_blank"
                    class=" font-light mx-auto relative after:absolute after:h-full after:w-full after:top-0 after:right-full after:bg-emerald-500 after:duration-200 hover:after:translate-x-full after:z-[-1] overflow-hidden"
                >
                    Create an account &rarr;
                </a>
            </div>

            <!-- <Step step={steps[0]}>
                <p>
                    Occassional Poetry is a <strong class="text-violet-400"
                        >React.js SPA</strong
                    >
                    styled with
                    <strong class="text-violet-400">TailwindCSS</strong>
                    that allows a user to generate poety. Input a recipient, the
                    style and feel of the poem, and have the
                    <strong class="text-violet-400">ChatGPT</strong> generate your
                    a perfect poem for any occasion.
                </p>
            </Step>
            <Step step={steps[1]}>
                <p>
                    Ultimate Todos is a Full Stack <strong
                        class="text-violet-400">Next.js</strong
                    >,
                    <strong class="text-violet-400">Node.js + Express.js</strong
                    >
                    & <strong class="text-violet-400">Firebase</strong> CRUD application
                    that allows a user to login, manage a tidy and efficacious todo
                    list, and persist this information across devices.
                </p>
            </Step>
            <Step step={steps[2]}>
                <p>
                    The exercises API is an public <strong
                        class="text-violet-400">JSON API</strong
                    >
                    serving up all types of exercise related information. The API
                    is a
                    <strong class="text-violet-400">Node.js + Express.js</strong
                    >
                    application served up by an
                    <strong class="text-violet-400">AWS EC2</strong> instance managed
                    through AWS Copilot.
                </p>
            </Step> -->
        </div>
    </section>
    <section
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24"
    >
        <!-- <div class="z-[-1] bg-violet-950 w-screen left-1/2 -translate-x-1/2 top-0 h-full absolute"> </div> -->
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-emerald-400 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-emerald-400 py-4 before:z-[-1] after:z-[-1]"
        >
            <h6 class="text-lg sm:text-xl md:text-2xl font-light">
                Ready for unlimited productivity?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Get started <span class="poppins text-emerald-400">today!</span>
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            To begin . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <!-- <div class="flex flex-col gap-2 mx-auto">
                    <div class="flex items-end gap-4">
                        <p
                            class="poppins text-6xl sm:text-7xl md:text-8xl text-slate-500 font-medium"
                        >
                            {benefit.metric}
                        </p>
                        <p
                            class="text-xl sm:text-2xl md:text-3xl capitalize pb-2"
                        >
                            {benefit.name}
                        </p>
                    </div>
                    <p class="text-center italic">- {benefit.description}</p>
                </div> -->
                <div class="flex gap-6 sm:gap-8">
                    <p
                        class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
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
        <div class="mx-auto pt-10">
            <button
                class="flex relative after:absolute after:bg-white after:bottom-0 after:right-full after:h-[1.5px] after:w-full hover:after:translate-x-full after:duration-200 overflow-hidden"
            >
                <p class="poppins z-10">
                    Start <span class="poppins text-emerald-400">chatting</span>
                    today &rarr;
                </p>
            </button>
        </div>

        <!-- <p class="mx-auto">To learn how to interact with <span class="text-emerald-400">Jasmine</span>, private message her the following message:</p> -->
    </section>
</main>
