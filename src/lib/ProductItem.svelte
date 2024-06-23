<script>
    // export let products;
    export let name;
    export let price;
    export let description;
    export let image;
    export let bgColour;
    export let shadow;
</script>

<main>
    <div class="item" style="background-color: {bgColour}; ">
        <img src={image} alt="" style="box-shadow: 7px 7px 7px -5px{shadow};" />

        <h2 style="text-shadow: 1.5px 1.5px{shadow};">{name}</h2>
        <h3 style="text-shadow: 1px 1px{shadow};">${price}</h3>
        <p style="text-shadow: 1px 1px{shadow};">{description}</p>
    </div>
</main>

<style>
    .item {
        margin: 15px;
        padding: 20px;
        border-radius: 5%;
    }

    img {
        height: 350px;
        border-radius: 3%;
    }

    h2 {
        font-family: "Red Hat Display", sans-serif;
        font-weight: 1000;
        color: #e8f2f6;
        font-size: 1.3rem;
    }

    h3 {
        font-family: "Red Hat Display", sans-serif;
        font-weight: 600;
        color: #e8f2f6;
        font-size: 1.2rem;
    }

    p {
        font-family: "Red Hat Display", sans-serif;
        font-weight: 500;
        color: #e8f2f6;
        font-size: 1.2rem;
    }
</style>
