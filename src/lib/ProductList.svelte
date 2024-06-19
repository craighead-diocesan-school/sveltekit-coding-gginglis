<script>
    import ProductItem from "$lib/ProductItem.svelte";
    let products = [
        {
            name: "pink sugar",
            price: 45,
            description: "pink tint",
        },
        {
            name: "vanilla beige",
            price: 46,
            description: "beige tint",
        },
        {
            name: "birthday cake",
            price: 47,
            description: "pink glitter tint",
        },
        {
            name: "brown sugar",
            price: 46,
            description: "caramel brown tint",
        },
    ];
</script>

<ProductItem />

<!-- <ul>
    {#each products as product, index}
        <li>
            {index + 1}. {product.name}, ${product.price},
            {product.description}
        </li>
    {/each}
</ul> -->
