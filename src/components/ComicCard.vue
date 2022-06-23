<template>
    <div class="comic-card">
        <div class="thumb-container">
            <img :src="imgUrl" :alt="cardTitle">
        </div>
        <p>{{ cardTitle }}</p>
    </div>
</template>

<script>
    export default{
        props: {
            imgUrl: String,
            cardTitle: String,
        },
        data(){
            return{};
        }
    }
</script>

<style lang="scss" scoped>
    .comic-card{
        cursor: pointer;
        color: whitesmoke;
        text-transform: uppercase;
        text-align: left;

        .thumb-container{
            aspect-ratio: 1 / 1;
            overflow: hidden;
        }

        p{
            padding-top: 1rem;
        }
    }
</style>