<template>
    <div>
        <div class="container">
            <TitleSection title="Current series" />
            <ul>
                <li v-for="(el, i) in Data" :key="i">
                    <Card :img="el.thumb" :text="el.series" />
                </li>
            </ul>
            <div class="btn-container">
                <div class="btn">
                    Load More
                </div>
            </div>
        </div>
    </div>
</template>

<script>
/* Import components */
import TitleSection from '../components/TitleSection.vue';
import Card from '../components/Card.vue';

/* Import data */
import Data from '../data/dc-comics';

export default {
    name: 'Content',
    components: {
        TitleSection,
        Card,
    },
    data() {
        return {
            Data,
        };
    },
}
</script>

<style scoped lang="scss">
@import "../styles/vars";

div {
    background: #1c1c1c;

    .container {
        color: #fff;

        ul {
            padding: 50px 0;
            list-style: none;
            display: flex;
            flex-wrap: wrap;

            li {
                width: calc(100% / 6);
                padding: 10px 5px;
                font-weight: 700;
            }
        }
    }
}

.btn-container {
    display: flex;
    justify-content: center;
}

.btn {
    display: inline-block;
    background: $primary-color;
    padding: 10px 60px;
    margin: 0 auto 50px;
    font-size: 16px;
    font-weight: 700;
    text-transform: uppercase;
    cursor: pointer;
}
</style>