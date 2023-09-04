<script>
    import "../app.css";
    import Footer from "../components/Footer.svelte";
    import Header from "../components/Header.svelte";
    export let y;
    let innerWidth = 0;
    let innerHeight = 0;
</script>

<Header {y} {innerHeight}/>
<section class=" uppercase font-medium bg-black border-b border-solid border-emerald-400 p-2 flex items-center justify-center">
    <p>First <span class="text-green-400">100</span> users get <span class="text-green-400">50%</span> more free tier</p>
</section>
<slot />
<Footer />

<svelte:window bind:scrollY={y} bind:innerHeight bind:innerWidth />
