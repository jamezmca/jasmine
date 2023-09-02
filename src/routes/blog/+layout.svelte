<section
    class="flex flex-col p-4 min-h-screen max-w-[1200px] w-full mx-auto gap-10"
>
    <header class="flex">
        <a class="font-medium" href="/">
            <h1>Try <span class="text-emerald-400">Jasmine</span></h1>
        </a>
    </header>
    <main
        class="flex flex-col mx-auto w-full max-w-[800px] gap-10 sm:gap-14 md:gap-20 font-light pb-20"
    >
        <slot />
    </main>
    <a
        href="/blog"
        class="flex mx-auto relative after:absolute mb-10 after:bg-white after:bottom-0 after:right-full after:h-[1.5px] after:w-full hover:after:translate-x-full after:duration-200 overflow-hidden"
    >
        <p class="poppins z-10">
            Back to <span class="poppins text-emerald-400">blogs</span>
        </p>
    </a>
</section>
