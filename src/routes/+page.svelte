<script>
    import ContactMe from "$lib/components/ContactMe.svelte";
    import Projects from "$lib/components/Projects.svelte";
    import SoftSkils from "$lib/components/SoftSkils.svelte";
    import Technologies from "$lib/components/Technologies.svelte";
    import Title from "$lib/components/Title.svelte";
    import Webkit from "$lib/components/Webkit.svelte";
    import Connections from "../lib/components/Connections.svelte";
</script>

<Webkit />

<main>
    <header class="container">
        <img class="profile-image" src="" alt="" />

        <title class="info">
            <h1 class="name">Fernando Carlos</h1>
            <h3 class="location">São Paulo, Brasil</h3>

            <p class="description">
                Olá sou desenvolvedor Front-end, tenho 20 anos, ultimamente
                tenho me dedicado, nas linguagens JavaScript e Typescript, em
                aprimorar minhas habilidades de resolução de problemas e em
                algumas tecnologias como Svelte, node.js e futuramente React com
                Tailwind. Estudo Programação voltada a Web a pouco mais de 1
                ano. Estou em busca de uma primeira oportunidade de estágio na
                area.
            </p>
        </title>
    </header>

    <Connections />

    <Title>Tecnologias</Title>

    <p class="notice">
        Atualmente essas são as tecnologias que utilizo para desenvolver meus
        projetos.
    </p>

    <div class="tech-container">
        <Technologies />
    </div>

    <Title>Soft Skills</Title>

    <SoftSkils />

    <Title>Projects</Title>

    <Projects />

    <Title>Deseja entrar em contato?</Title>

    <ContactMe />

    <footer>
        <p>&copy; Fernando Carlos. All rigths reserved</p>
    </footer>
</main>

<style>
    @import url("https://fonts.googleapis.com/css2?family=Roboto:wght@700&display=swap");
    :global(body) {
        margin: 0;
        background: rgb(11, 11, 11);
    }

    main {
        font-family: "Roboto", sans-serif;
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
        color: #ffffff;
    }

    .description {
        margin-top: 0px;
        width: 580px;
        font-size: 18.5px;
        color: #ffffffa8;
    }

    .tech-container {
        display: flex;
        justify-content: center;
    }

    .notice {
        display: flex;
        justify-content: center;
        font-size: 23px;
        color: #ffffffa8;
        margin-bottom: 40px;
    }

    footer{
        color: #ffff;
        font-size: 18px;
    }
</style>
