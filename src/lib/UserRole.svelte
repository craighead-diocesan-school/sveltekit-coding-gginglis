<script>
    let role = "";
</script>

<input bind:value={role} placeholder="what is your role" />

{#if role == "admin"}
    <h1>welcome, admin!</h1>
    <h2>you have full access</h2>
{:else if role == "editor"}
    <h1>welcome, editor!</h1>
    <h2>you can edit but your access is limited</h2>
{:else if role == "guest"}
    <h1>welcome, guest</h1>
    <h2>you can view only</h2>
{:else}
    <h1>welcome, user!</h1>
    <h2>your access is limited</h2>
{/if}

<style>
    h1,
    h2 {
        display: flex;
        flex-direction: column;
        margin-left: 30px;
        font-weight: bold;
        font-size: 1.2rem;
        color: rgb(38, 41, 116);
        font-family: "Red Hat Display", sans-serif;
    }

    input {
        margin-left: 30px;
        border: solid rgb(38, 41, 116) 3px;
    }
</style>
