<template>
    <div>
        <div class="img">
            <img :src="img" :alt="text">
        </div>
        <span>{{ text }}</span>
    </div>
</template>

<script>
export default {
    name: 'Card',
    props: {
        img: String,
        text: String,
        columns: Number,
    },
}
</script>

<style scoped lang="scss">
div {
    display: flex;
    flex-direction: column;

    .img {
        max-height: 185px;
        overflow: hidden;
    }

    .img img {
        display: block;
        width: 100%;
    }

    span {
        padding: 20px 0;
        font-size: 16px;
        text-transform: uppercase;
    }
}
</style>