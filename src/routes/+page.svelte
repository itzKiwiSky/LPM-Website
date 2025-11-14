<script>
    import TopBar from "../components/TopBar.svelte";

</script>
<style>
    .container
    {
        background-color: #260f3a;
        height: 100vh;
        color: white;
    }

    .center-page
    {
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
    }

    .cat-deco
    {
        image-rendering: pixelated;
        width: 30%;
    }

</style>

<div class="container">
    <TopBar/>
    <div class="center-page">
        <img src="cat_pixel.gif" alt="" class="cat-deco">
        <h1>Criando universos desde 2025</h1>
    </div>
</div>