<script>
    import { page } from "$app/stores";
    // console.log($page?.url?.searchParams.get("user_id"));
    let cancelStatus = null;
    let user_id;

    async function handleCancelSubscription() {
        if (cancelStatus === "cancelling" || !user_id) {
            return;
        }
        try {
            const cancelURL =
                "https://jasmine-api.onrender.com/api/cancel_subscription?user_id=" +
                user_id.replaceAll("#", "%23");

            console.log(cancelURL);
            const res = await fetch(cancelURL)
            if (res.status === 200) {
                cancelStatus = 'cancelled'
            } else {
                cancelStatus = null
            }
        } catch (err) {
            cancelStatus = null;
        }
    }

    $: {
        user_id =
            $page?.url?.searchParams.get("user_id") + ($page?.url?.hash || "");
    }
</script>

<main
    class="mx-auto max-w-[1000px] w-full p-4 sm:p-6 flex-1 flex flex-col justify-center items-center"
>
    <section
        class="flex flex-col gap-4 sm:gap-6 md:gap-8 overflow-hidden max-w-full"
    >
        <h1
            class="text-4xl sm:text-5xl md:text-6xl font-semibold text-center truncate"
        >
            {user_id}
        </h1>
        <!-- <p class="opacity-80 mx-auto"><strong>User</strong> {"1"}</p> -->

        {#if cancelStatus === "cancelled"}
            <p class="text-center max-w-[500px] mx-auto w-full font-light">
                Your subscription has been cancelled! You can still interact
                with Jasmine within the bounds of a free user account :)
            </p>
            <a
                href="/"
                class="flex mx-auto relative after:absolute after:bg-white after:bottom-0 after:right-full after:h-[1.5px] after:w-full hover:after:translate-x-full after:duration-200 overflow-hidden"
            >
                <p class="poppins z-10">
                    Back <span class="poppins text-emerald-400">home</span>
                    <i class="fa-solid fa-home" />
                </p>
            </a>
        {:else if cancelStatus === "cancelling"}
            <div class="flex items-center gap-4 mx-auto font-light">
                <p>Cancelling</p>
                <i class="fa-solid fa-spinner animate-spin" />
            </div>
        {:else}
            <p class="mx-auto text-base sm:text-lg text-center">
                Are you sure you want to <span class="poppins text-amber-400"
                    >cancel</span
                > your subscription?
            </p>
            <div class="flex items-center gap-4 mx-auto">
                <a
                    href="/"
                    class="border border-solid border-emerald-400 bg-emerald-950 duration-200 hover:bg-emerald-900 px-4 py-2 rounded-md"
                    >Cancel</a
                >
                <button
                    on:click={handleCancelSubscription}
                    class="border border-solid border-amber-400 bg-amber-950 duration-200 hover:bg-amber-900 px-4 py-2 rounded-md"
                    >Confirm</button
                >
            </div>
        {/if}

        <!-- <a
            href="/"
            class="flex mx-auto relative after:absolute after:bg-white after:bottom-0 after:right-full after:h-[1.5px] after:w-full hover:after:translate-x-full after:duration-200 overflow-hidden"
        >
            <p class="poppins z-10">
                Back <span class="poppins text-emerald-400">home</span>
                <i class="fa-solid fa-home" />
            </p>
        </a> -->
    </section>
</main>
