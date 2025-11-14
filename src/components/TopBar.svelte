<style>
    @keyframes bounceInOut {
        0% {
            transform: translateY(0);
        }
        25% {
            transform: translateY(-3%);
        }
        50% {
            transform: translateY(0);
        }
        75% {
            transform: translateY(-3%);
        }
        100% {
            transform: translateY(0);
        }
    }

    .container 
    {
        background: transparent;
    }

    .topbar-container 
    {
        position: fixed;
        background-color: black;
        display: flex;
        align-items: center;

        clip-path: polygon(0% 0%, 80% 0%, 70% 100%, 0% 100%);
    }

    .logo-topbar 
    {
        max-width: 12%;
        height: auto;
        transition: 0.3s;
    }

    .logo-topbar:hover {
        animation: bounceInOut 1s ease-in-out;
    }

    .navbar
    {
        width: 60%;
    }

    .navbar a
    {
        text-align: center;
        color: white;
        text-decoration: none;
        font-size: 165%;
        padding-left: 2%;
        padding-right: 2%;
        transition: 0.5s;
    }

    .navbar a:hover
    {
        text-shadow: 0 0 20px white;
    }

    /* responsive tweaks - reduce sizes on small screens */
    @media (max-width: 800px) 
    {
        .logo-topbar { width: 20%; }
    }

    @media (max-width: 420px) 
    {
        .logo-topbar { width: 28%; }
    }
</style>

<div class="container">
    <div class="topbar-container">
        <img src="logo_lpm_placeholder.svg" alt="" class="logo-topbar">
        <nav class="navbar">
            <a href="#about">Sobre Nos</a>
            <a href="#">Integrantes</a>
            <a href="#">Projetos</a>
            <a href="#">Assets</a>
        </nav>
    </div>
</div>