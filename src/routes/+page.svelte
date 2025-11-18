<script>
    import About from "../components/About.svelte";
    import Separator from "../components/Separator.svelte";

</script>
<style>
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

<div class="center-page">
    <img src="cat_pixel.gif" alt="" class="cat-deco">
    <h1 style="text-shadow: 0 0 30px white">Criando universos desde 2025</h1>
</div>
<Separator linewidth={0.5} sepmargin={5}/>
<About/>