<script lang="ts">
    import logos from "$lib/json/lang-logos.json";
</script>

<div class="techs">
    {#each logos as logos (logos.alt)}
        <div class="svg-techs {logos.class}">
            <img
                class="logos"
                src="/technologies/{logos.src}"
                alt={logos.alt}
            />
        </div>
    {/each}
</div>

<style>
    .techs {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
        background: none;
        width: 60%;
    }

    .svg-techs {
        justify-content: center;
        display: inline-flex;
        width: 100px;
        height: 100px;
        border-radius: 15px;
        margin: 15px;
    }

    .logos {
        width: 90px;
    }

    .html,
    .svelte,
    .git {
        border: 1px solid #e44d26;
    }

    .css {
        border: 1px solid #1172b8;
    }

    .js {
        border: 1px solid #f7df1e;
    }

    .ts {
        border: 1px solid #3178c6;
    }

    .node {
        border: 1px solid #8cc84b;
    }

    .bootstrap {
        border: 1px solid #563d7c;
    }
</style>
