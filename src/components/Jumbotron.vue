<template>
    <div class="jumbotron">
        <img :src="require(`../assets/${img}`)" alt="Jumbotron">
    </div>
</template>

<script>
export default {
    name: 'Jumbotron',
    props: {
        img: String,
    },
}
</script>

<style scoped lang="scss">
.jumbotron {
    height: 500px;
    overflow: hidden;

    img {
        width: 100%;
    }
}

</style>