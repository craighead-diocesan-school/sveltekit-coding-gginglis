<script>
    export let products = [];
</script>

<ul>
    {#each products as product (product.name)}
        <li>
            {product.name}, ${product.price},
            {product.description}
        </li>
    {/each}
</ul>
