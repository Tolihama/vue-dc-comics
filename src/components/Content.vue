<template>
    <div>
        <div class="container">
            {{ content }}
        </div>
    </div>
</template>

<script>
export default {
    name: 'Content',
    data() {
        return {
            content: '--> Content goes here <--',
        };
    },
}
</script>

<style scoped lang="scss">
div {
    background: #1c1c1c;

    .container {
    padding: 50px 0;
    color: #fff;
    font-size: 30px;
    font-weight: 700;
    }
}
</style>