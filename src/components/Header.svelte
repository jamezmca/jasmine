<script>
    export let y;
    export let innerHeight;
</script>

<header
    class={"top-0 left-1/2 -translate-x-1/2 w-full flex flex-col max-w-[1200px] mx-auto fixed duration-200 p-4 sm:p-6 " +
        (y > 0
            ? " pointer-events-auto opacity-100"
            : " pointer-events-none opacity-0")}
>
    <div
        class="flex flex-col-reverse sm:flex-row sm:items-center gap-2  ml-auto"
    >

        <a
            href="/blog"
            class="rounded-full border border-solid border-emerald-950 bg-slate-950 ml-auto px-4 py-2 flex items-center gap-2 duration-200 hover:border-emerald-600 z-[50] relative"
        >
            <h1>
                Blog
            </h1>
        </a>
        <a
            href="https://discord.gg/VRxj4gbjVQ"
            target="_blank"
            class="rounded-full border border-solid border-emerald-950 bg-slate-950 ml-auto px-4 py-2 flex items-center gap-2 duration-200 hover:border-emerald-600 z-[50] relative"
        >
            <h1>
                Start <span class="poppins text-emerald-400">chatting</span> today
            </h1>
            <i class="fa-brands fa-discord" />
        </a>
    </div>
</header>
