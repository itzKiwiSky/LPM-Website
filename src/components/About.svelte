<style> 
    :root {
        --bg-color: rgb(84, 40, 134);
    }

    .wave-section {
        position: relative;
        overflow: hidden; /* importante */
    }

    /* Conteúdo normal dentro */
    .wave-section .content {
        padding: 4% 2%;
        display: flex;        /* você pode tirar ou trocar */
        justify-content: center;
        align-items: center;
        flex-direction: column;
        background-color: var(--bg-color);
    }

    /* A onda (top e bottom) */
    .wave {
        width: 100%;
        height: 62px; /* mesmo da sua SVG */
        background: var(--bg-color); /* cor da onda (ou gradient) */
        clip-path: polygon(
        7.14% 0%,
        3.57% 50%,
        0% 100%,
        7.14% 100%,
        14.29% 100%,
        17.85% 100%,
        25% 100%,
        28.57% 100%,
        35.71% 100%,
        39.29% 100%,
        46.43% 100%,
        50% 100%,
        57.14% 100%,
        60.71% 100%,
        67.85% 100%,
        71.43% 100%,
        78.57% 100%,
        82.14% 100%,
        89.28% 100%,
        92.85% 100%,
        100% 100%,
        96.42% 50%,
        92.82% 0%,
        89.28% 50%,
        87.5% 75%,
        85.71% 50%,
        82.14% 0%,
        78.57% 50%,
        76.78% 75%,
        75% 50%,
        71.42% 0%,
        67.85% 50%,
        66.07% 75%,
        64.28% 50%,
        60.71% 0%,
        57.14% 50%,
        55.35% 75%,
        53.57% 50%,
        50% 0%,
        46.42% 50%,
        44.64% 75%,
        42.85% 50%,
        39.28% 0%,
        35.71% 50%,
        33.92% 75%,
        32.14% 50%,
        28.57% 0%,
        25% 50%,
        23.21% 75%,
        21.42% 50%,
        17.85% 0%,
        14.28% 50%,
        12.5% 75%,
        10.71% 50%
        );
    }

    .wave.top
    {
        transform: translateY(0.5px);
    }

    /* Inverter para a onda de baixo */
    .wave.bottom {
        transform: rotate(180deg);
    }

    .content
    {
        text-shadow: 0 0 30px white;

        & h1
        {
            font-size: 240%;
            margin-bottom: 1.5%;
        }

        & p
        {
            font-size: 140%;
        }
    }
</style>

<div class="container">
    <div class="wave-section">
        <div class="wave top"></div>

        <div class="content" id="about">
            <h1>Sobre nos</h1>
            <p>Somos um grupo formado por 3 estudantes de jogos digitais</p>
            <p>ainda em inicio de carreira.</p>
        </div>

        <div class="wave bottom"></div>
    </div>
</div>