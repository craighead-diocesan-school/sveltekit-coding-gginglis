<script>
    let ImageUrl = "https://picsum.photos/200";
    let caption = "fire emoji";
    let linkUrl = "https://www.google.com";
</script>

<figure>
    <a href={linkUrl}>
        <img src={ImageUrl} alt="" />
    </a>
    <figcaption>{caption}</figcaption>
</figure>

<style>
    figure {
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 1rem;
        padding: 1.5rem;
        width: fit-content;
        border-radius: 10px;
        box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
        backdrop-filter: blur(4px);
        background: rgba(98, 217, 255, 0.25);
    }
</style>
