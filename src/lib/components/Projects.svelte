<script>
    import projects from "$lib/json/projects.json";
</script>

<div class="container">
    {#each projects as projects}
        <div class="projects">
            <div class="conteudo">
                <h1>{projects.title}</h1>
                <p>{projects.description}</p>
            </div>

            <button>
                <a href={projects.link} target="_blank">Vizualizar projeto</a>
            </button>
        </div>
    {/each}
</div>

<style>
    .container {
        display: flex;
        justify-content: center;
        align-items: start;
        flex-wrap: wrap;
        flex-direction: row;
        width: 90%;
    }

    .projects {
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        width: 400px;
        height: 250px;
        margin: 20px;
        border: 2px solid rgba(199, 19, 88, 0.479);
        border-radius: 15px;
    }

    .projects:hover {
        border: 2px solid rgb(255, 0, 98);
    }

    .conteudo {
        height: 180px;
        width: 90%;
        margin: 10px;
    }

    h1 {
        margin: 10px;
        text-align: center;
        color: #ffff;
    }

    p {
        font-size: 20px;
        margin: 10px;
        color: #ffffffa8;
    }

    a {
        text-decoration: none;
        color: rgba(204, 0, 255, 0.603);
    }

    a:hover {
        font-size: 21px;
        color: rgb(204, 0, 255);
    }

    button {
        width: 200px;
        display: inline-block;
        font-size: 20px;
        height: 50px;
        border: none;
        background: none;
    }
</style>
