<script>
    import Header from "$lib/Header.svelte";
    import Footer from "$lib/Footer.svelte";
    import ImageCard from "../lib/ImageCard.svelte";
    import HiButton from "../lib/HiButton.svelte";
</script>

<Header />

<main>
    <HiButton />
    <ImageCard />
</main>

<Footer />

<style>
    main {
        display: flex;
    }
</style>
