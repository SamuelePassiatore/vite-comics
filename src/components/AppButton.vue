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
}
</style>