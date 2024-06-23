<script>
    import ProductItem from "$lib/ProductItem.svelte";
    let products = [
        {
            name: "cherry",
            price: 45,
            description: "red tint",
            image: "/cherry.jpg",
            bgColour: "#c45d56",
            shadow: "#5B130E",
        },
        {
            name: "pink sugar",
            price: 45,
            description: "pink tint",
            image: "/pink-sugar.jpg",
            bgColour: "#d98f95",
            shadow: "#C66569",
        },
        {
            name: "sweet mint",
            price: 45,
            description: "freshhh",
            image: "/sweet-mint.jpg",
            bgColour: "#C0D1A2",
            shadow: "#BBC6A1",
        },
        {
            name: "vanilla beige",
            price: 45,
            description: "beige tint",
            image: "/vanilla-beige.jpg",
            bgColour: "#b38c7f",
            shadow: "#70453A",
        },
    ];
</script>

<main>
    {#each products as product (product.name)}
        <ProductItem {...product} />
    {/each}
</main>

<style>
    main {
        display: flex;
    }
</style>
