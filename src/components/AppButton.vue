<script>
export default {
    name: 'App Button',
    props: {
        text: String
    }
}
</script>

<template>
    <button>{{ text }}</button>
</template>

<style lang="scss" scoped>
button {
    padding: 8px 30px;
    background-color: dodgerblue;
    border: transparent;
    color: white;
    text-transform: uppercase;
    cursor: pointer;
    margin: 10px 0;

    &:hover {
        box-shadow: 1px 0 10px white;
    }
}
</style>