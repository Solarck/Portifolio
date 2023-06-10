<script>
    import Technologies from "$lib/components/Technologies.svelte";
    import Connections from "../lib/components/Connections.svelte";
</script>

<main>
    <header class="container">
        <img class="profile-image" src="" alt="" />

        <title class="info">
            <h1 class="name">Fernando Carlos</h1>
            <h3 class="location">São Paulo, Brasil</h3>

            <p class="description">
                Olá sou desenvolvedor Front-end, tenho 20 anos, ultimamente
                tenho me dedicado, nas linguagens JavaScript e Typescript, em
                aprimorar minhas habilidades de resolução de problemas e
                Frameworks como Svelte (por curiosidade) e futuramente React.
                Estudo Programação voltada a Web a pouco mais de 1 ano. Estou,
                aberto e em, busca de uma primeira oportunidade de estágio na
                area.
            </p>
        </title>
    </header>

    <Connections />

    <div class="title-tech">
        <h3 class="title">Tecnologias</h3>
    </div>

    <p class="notice">
        Atualmente essas são as tecnologias que utilizo para desenvolver meus
        projetos.
    </p>

    <div class="tech-container"><Technologies /></div>
</main>

<svelte:head>
    <title>Solarck | Portifolio</title>

    <style>
        ::-webkit-scrollbar {
            width: 13px;
        }

        ::-webkit-scrollbar-track {
            background: rgb(48, 46, 46);
            border-radius: 50px;
        }

        ::-webkit-scrollbar-thumb {
            background: rgba(223, 84, 137, 0.349);
            border-radius: 50px;
        }

        ::-webkit-scrollbar-thumb:hover {
            background: rgba(223, 84, 137, 0.884);
        }

        /* © Fernando Carlos. All rigths reserved */
    </style>
</svelte:head>

<style>
    :global(body) {
        margin: 0;
        background: rgb(11, 11, 11);
    }

    main {
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        width: 1000px;
        height: 100%;
    }

    header {
        display: flex;
        flex-wrap: wrap;
        align-items: center;
        justify-content: start;
        flex-direction: column;
        width: 90%;
        height: 450px;
        margin-left: 10px;
    }

    .profile-image {
        display: flex;
        margin-top: 100px;
        width: 260px;
        height: 245px;
        border-radius: 10px;
        border: 2px solid #ffff;
        background: rgb(11, 11, 11);
    }

    .info {
        display: flex;
        flex-direction: column;
    }

    .name {
        margin: 100px 0px 0px 0px;
        font-size: 35px;
        color: rgb(240, 11, 99);
    }

    .location {
        margin-top: 5px;
        font-size: 25px;
        color: #ffffffa8;
    }

    .description {
        margin-top: 0px;
        width: 580px;
        font-size: 18px;
        color: #ffffff;
    }

    .tech-container {
        display: flex;
        justify-content: center;
    }

    .title-tech {
        display: flex;
        flex-direction: row;
        margin: 80px 0px 10px 0px;
        font-size: 35px;
        color: #ffff;
    }

    .title {
        color: rgb(240, 11, 99);
        margin: 0px;
        display: inline-block;
    }

    .notice {
        display: flex;
        justify-content: center;
        font-size: 23px;
        color: #ffffffa8;
        margin-bottom: 40px;
    }
</style>
