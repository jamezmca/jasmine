<script>
    let blogs = [
        {
            name: "How to use Discord to improve your organization.",
            description:
                "Finding a good organizational system is an age old system; there's always a new app, or a new diary, or maybe even a whiteboard. This issue with these options is that it adds an additional item to you way of life that you have to manage. With Discord, organization comes build in to an app that we already use, meaning there's no downloads, no extra stuff to manage; it's as simeple as having a personal assistant.",
            href: "/blog/how_to_use_discord_for_organization",
        },
    ];
</script>

<h1 class="text-center text-4xl sm:text-5x md:text-6xl font-semibold">
    Blog Articles
</h1>
<div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
    {#each blogs as blog, index}
        <a href={blog.href} class="flex gap-6 sm:gap-8 group cursor-pointer">
            <p
                class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
            >
                0{index + 1}
            </p>
            <div class="flex flex-col gap-6 sm:gap-8">
                <h3
                    class="text-2xl sm:text-3xl md:text-5xl group-hover:text-emerald-400 duration-200"
                >
                    {blog.name}
                </h3>
                <p class="font-light">{blog.description}</p>
            </div>
        </a>
    {/each}
</div>

<svelte:head>
    <title>Try Jasmine · Blog</title>
</svelte:head>
