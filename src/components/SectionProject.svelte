<script lang="ts">
    let { imgsrc, bgcol, fgcol, title, desc, direction } = $props();
</script>

<style>
    .container
    {
        margin-top: 2%;
    }

    .colored-div
    {
        padding: 2%;
        display: flex;

        & img
        {
            width: 10%;
        }
    }

    .text-div
    {
        display: flex;
        margin-left: 4%;
        margin-right: 4%;
        flex-direction: column;
        text-align: --direction;
        width: 100%;

        & h2
        {
            margin-bottom: 2%;
        }

        & .text-title
        {
            font-size: 350%;
            text-shadow: 0 0 20px white;
        }

        & .text-desc
        {
            font-size: 200%;
            text-shadow: 0 0 20px white;
        }
    }

</style>

<div class="container">
    <div class="colored-div" style="background-color: {bgcol}; color: {fgcol}; justify-content: {direction}">
        <img src={imgsrc} alt="">
        <div class="text-div">
            <h2 class="text-title">{title}</h2>
            <h2 class="text-desc">{desc}</h2>
        </div>
    </div>
</div>