<script lang="ts">
    export let tag: "h1" | "h2" | "h3";
</script>

<svelte:element this={tag} class="titulo tag-{tag}">
    <slot />
</svelte:element>

<style>
    .container {
        display: flex;
        justify-content: center;
        text-align: center;
    }

    .tag-h1,
    .tag-h2 {
        display: inline-block;
        color: rgb(240, 11, 99);
        margin: 80px 0px 20px 0px;
        font-size: 40px;
        text-align: center;
    }

    @media screen and (max-width: 750px) {
        .tag-h2 {
            margin: 490px 0px 20px 0px;
        }
    }
</style>
