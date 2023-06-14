<div class="container">
    <h3 class="title"><slot /></h3>
</div>

<style>
    .container {
        display: flex;
        justify-content: center;
    }

    .title {
        display: inline-block;
        color: rgb(240, 11, 99);
        margin: 80px 0px 20px 0px;
        font-size: 40px;
    }
</style>
