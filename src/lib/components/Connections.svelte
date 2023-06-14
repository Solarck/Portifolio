<script lang="ts">
    import icons from "$lib/json/icons.json";
</script>

<nav class="social-media">
    <h1>Conexões:</h1>

    {#each icons as icons (icons.alt)}
        <button class="icon">
            <a href={icons.href} target="_blank">
                <img src="/icons/{icons.src}" alt={icons.alt} />
            </a>
        </button>
    {/each}
</nav>

<style>
    .social-media {
        display: flex;
        justify-content: start;
        flex-direction: row;
        width: 95%;
        margin-top: -90px;
    }

    .icon {
        border: none;
        width: 46px;
        height: 0%;
        background: rgb(11, 11, 11);
        margin-left: 3px;
    }

    h1 {
        margin: 10px 0px 0px 55px;
        padding-bottom: 20px;
        display: inline-block;
        color: #fff;
    }

    .icon:hover {
        width: 54px;
    }
</style>
