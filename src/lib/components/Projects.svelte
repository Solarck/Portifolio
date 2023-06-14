<script>
    import projects from "$lib/json/projects.json";
</script>

<div class="container">
    {#each projects as projects}
        <div class="projects">
            <div class="conteudo">
                <h1>{projects.title}</h1>
                <p>{projects.description}</p>

                <div class="tags">
                    <h4>{projects.tag1}</h4>
                    <h4>{projects.tag2}</h4>
                    <h4>{projects.tag3}</h4>
                </div>

                <button>
                    <a href={projects.link} target="_blank">Vizualizar projeto</a>
                </button>
            </div>
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
        height: 800px;
    }

    .projects {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 400px;
        height: 320px;
        margin: 20px;
        border: 2px solid rgba(199, 19, 88, 0.479);
        border-radius: 15px;
    }

    .projects:hover {
        border: 2px solid rgb(255, 0, 98);
    }

    .conteudo {
        margin: -100px 5px 0px 0px;
        height: 180px;
        width: 90%;
    }

    h1 {
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
        color:  rgb(204, 0, 255);
    }

    .tags {
        width: 100%;
        height: 50px;
        display: flex;
    }

    h4 {
        font-size: 18px;
        color: rgba(0, 132, 255, 0.726);
        margin: 10px 5px 0px 10px;
    }

    button {
        width: 200px;
        font-size: 20px;
        height: 50px;
        margin: 10px 0px 0px -12px;
        border: none;
        background: none;
    }
</style>
