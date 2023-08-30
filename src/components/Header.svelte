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
    <button
        class="rounded-full border border-solid border-emerald-950 bg-slate-950 ml-auto px-4 py-2 flex items-center gap-2 duration-200 hover:border-emerald-600 z-[50] relative"
    >
        <h1>
            Start <span class="poppins text-emerald-400">chatting</span> today
        </h1>
        <i class="fa-brands fa-discord" />
    </button>
</header>
