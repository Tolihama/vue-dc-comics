<template>
    <div class="title">
        {{ title }}
    </div>
</template>

<script>
export default {
    name: 'TitleSection',
    props: {
        title: String,
    },

}
</script>

<style scoped lang="scss">
@import "../styles/vars";

div.title {
    display: inline-block;
    position: absolute;
    transform: translateY(-50%);
    background: $primary-color;
    padding: 10px 30px;
    font-size: 24px;
    font-weight: 700;
    color: #fff;
    text-transform: uppercase;
}
</style>