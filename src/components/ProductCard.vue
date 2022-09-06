<template>
            <div class="card">
                <div class="card-image">
                    <img :src="img" :alt="title">
                </div>
                <div class="card-text">{{title}}</div>
            </div> 

</template>

<script>
export default {
    props: {
        img: String,
        title: String,
        price: String,
        type: String
    }
}
</script>

<style lang="scss" scoped>

    .card{
        .card-image{
            width: 100%;
            height: 200px;
            aspect-ratio: 1;
            overflow: hidden;
        }
        .card-text{
            padding: 10px 0;
            color: white;
            text-transform: uppercase;
        }
    }

</style>