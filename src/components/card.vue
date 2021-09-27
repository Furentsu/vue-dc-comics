<template>
    <div class="card">
        <a href="#">
            <img :src="seriesImage" alt="Series image"/>
            <h4>{{seriesName}}</h4>
        </a>
    </div>
</template>

<script>
export default {
    name: 'card',
    props: ['seriesImage','seriesName'],
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

    .card {
        flex-basis: calc(100% / 6);
        text-align: center;

        img {
            height: 75%;
        }

        h4 {
            padding: 10px;
            color: white;
        }
    }
</style>