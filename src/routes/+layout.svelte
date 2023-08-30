<script>
    import "../app.css";
    import Footer from "../components/Footer.svelte";
    import Header from "../components/Header.svelte";
    export let y;
    let innerWidth = 0;
    let innerHeight = 0;
</script>

<Header {y} {innerHeight}/>
<slot />
<Footer />

<svelte:window bind:scrollY={y} bind:innerHeight bind:innerWidth />
