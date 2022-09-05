<template>
    <main>

        <div class="container">
            <div> --> Content goes here  </div>
        </div>

    </main>
</template>

<script>
export default {
    name: 'MainContent'
}
</script>

<style lang="scss" scoped>

    @import '../style/variables.scss';

main {
    background-color: $main-content-bg;
    height: 150px;

    .container{
        display: flex;
        align-items: center;
        color: white;
        font-size: 30px;
    }
}
</style>