<script>
export default {
    name: 'Series Card',
    props: {
        card: Object
    }
}
</script>

<template>
    <div class="series-card">
        <img :src="card.thumb" :alt="card.thumb">
        <h6>{{ card.series }}</h6>
    </div>
</template>

<style lang="scss" scoped>
.series-card {
    flex-basis: calc(100% / 6);
    padding: 15px;

    img {
        display: block;
    }

    h6 {
        text-transform: uppercase;
        padding-top: 10px;
    }
}
</style>