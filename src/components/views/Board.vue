<template>

<section>
    <h3>
        <span>
            Mis Paneles > {{ name }}
        </span>
    </h3>
    <div>
        ...
    </div>
</section>

</template>

<script>

const Board = {
    name: 'board',
    components: {},
    props: {
        name: String,
        id: Number
    }
}

export default Board;
</script>

<style lang="scss" scoped>
    section {
        text-align: left;
    }

    h3 {
        color: #37474f;
        text-align: left;
        margin: 1.5rem;
    }

    span {
        color: #546e7a;
    }

</style>