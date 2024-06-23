<script>
    import Header from "$lib/Header.svelte";
    import ProductList from "$lib/ProductList.svelte";
    import Footer from "$lib/Footer.svelte";
</script>

<body>
    <Header />

    <h2>summer fridays</h2>
    <ProductList />

    <Footer />
</body>

<style>
    body {
        background-color: #e8f2f6;
    }

    h2 {
        font-family: "Red Hat Display", sans-serif;
        font-weight: 1000;
        font-size: 1.7rem;
        color: rgb(38, 41, 116);
        margin: 30px;
    }
</style>
