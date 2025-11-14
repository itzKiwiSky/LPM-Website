<script lang="ts">
    export let linewidth: number = 0.5;   // valor padrão
    export let sepmargin: number = 5;   // valor padrão
</script>

<style>
    .container
    {
        display: flex;
        justify-content: center;
    }
    .separator
    {
        margin-top: var(--sepmargin);
        margin-bottom: var(--sepmargin);
        min-height: var(--linewidth);
        min-width: 75%;
        background-color: transparent;
        background: linear-gradient(90deg,rgba(38, 15, 58, 0) 0%, rgba(112, 75, 148, 0.75) 25%, rgba(170, 110, 230, 1) 50%, rgba(112, 75, 148, 0.75) 75%, rgba(38, 15, 58, 0) 100%);
        background-size: cover;
        background-position: center;
    }
</style>

<div class="container">
    <div class="separator" style=" --linewidth: {linewidth}vh; --sepmargin: {sepmargin}%; "></div>
</div>