<script lang="ts">
    import favicon from '$lib/assets/favicon.svg';

    import About from "../components/About.svelte";
    import Footer from "../components/Footer.svelte";
    import Separator from "../components/Separator.svelte";
    import TopBar from "../components/TopBar.svelte";

    let { children } = $props();
</script>

<svelte:head>
    <link rel="icon" href={favicon} />
</svelte:head>

<style>
    .container
    {
        background-color: #260f3a;
        height: 100%;
        min-height: 100vh;
        color: white;
    }

</style>

<div class="container">
    <TopBar/>
    {@render children()}
    <Footer/>
</div>
