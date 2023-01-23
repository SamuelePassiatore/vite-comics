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
    position: relative;
    transition: box-shadow 1s;
    cursor: pointer;

    &:hover {
        box-shadow: inset 1px 0 10px white;
    }

    img {
        display: block;
        height: 140px;
        width: 140px;
    }

    h6 {
        text-transform: uppercase;
        padding-top: 10px;
    }
}
</style>