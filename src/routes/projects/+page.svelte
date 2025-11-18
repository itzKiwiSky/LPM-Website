<script lang="ts">
    import SectionProject from "../../components/SectionProject.svelte";

    type Game = {
        imgsrc: string,
        title: string,
        desc: string,
        bgcol: string,
        fgcol: string,
        direction: string,
    }

    let games: Array<Game> = [
        {
            imgsrc: "icon.png",
            title: "Jogo do coco 2",
            desc: "Ainda e um jogo sobre um coco tlgd",
            bgcol: "#323232",
            fgcol: "#ffffff",
            direction: "",
        },
        {
            imgsrc: "icon.png",
            title: "Jogo do coco 2",
            desc: "Ainda e um jogo sobre um coco tlgd",
            bgcol: "#323232",
            fgcol: "#ffffff",
            direction: "",
        },
        {
            imgsrc: "icon.png",
            title: "Jogo do coco 2",
            desc: "Ainda e um jogo sobre um coco tlgd",
            bgcol: "#323232",
            fgcol: "#ffffff",
            direction: "",
        },
        {
            imgsrc: "icon.png",
            title: "Jogo do coco 2",
            desc: "Ainda e um jogo sobre um coco tlgd",
            bgcol: "#323232",
            fgcol: "#ffffff",
            direction: "",
        },
    ]
</script>

<style>
    .container
    {
        padding-top: 10%;
    }
    
    h1
    {
        text-align: center;
        font-size: 400%;
        text-shadow: 0 0 30px white;
        color: white;
    }
</style>

<div class="container">
    <h1>Nossos projetos</h1>
    {#each games as game, i}
        <SectionProject direction={i % 2 === 0 ? "right" : "left"} imgsrc={game.imgsrc} bgcol={game.bgcol} fgcol={game.fgcol} title={game.title} desc={game.desc}/>
    {/each}
</div>