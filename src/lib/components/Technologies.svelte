<script lang="ts">
    import logos from "$lib/json/lang-logos.json";
</script>

<div class="techs">
    {#each logos as logos (logos.alt)}
        <div class="svg-techs">
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
        background: rgb(11, 11, 11);
        width: 60%;
    }

    .svg-techs {
        justify-content: center;
        display: inline-flex;
        width: 100px;
        height: 100px;
        border-radius: 15px;
        border: 1px solid rgba(240, 11, 99, 0.521);
        margin: 15px;
    }

    .svg-techs:hover {
        border: 1px solid rgb(240, 11, 99);
    }

    .logos {
        width: 90px;
    }
</style>
