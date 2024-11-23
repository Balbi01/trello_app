<template>
<ul>
    <li
        v-for="(task, index) in tasks"
        :key="index"
        :class="{ completed: task.completed }">
        {{ task.title }}
    </li>

    <input type="text"
        placeholder="Añadir nueva tarea"
        v-model="title"
        @keyup.enter="add()"
    >
</ul>
</template>

<script>
const TaskList = {
    name: 'TaskList',

    props: {
        listId: String,
        tasks: Array
    },

    data() {
        return {
            title: ''
        }
    },

    methods: {
        add() {
            // TODO
        }
    }
}

export default TaskList;
</script>

<style lang="scss" scoped>
ul {
    list-style: none;
    margin: 0;
    padding: 0;
}

li {
    background-color: #fAFAFA;
    border-radius: 3px;
    border-bottom: 1px solid #CCC;
    margin: 0.25rem 0;
    padding: 1rem;

    &.completed {
        background-color: #CFD8DC;
        color: #90A4AE;
    }
}

</style>