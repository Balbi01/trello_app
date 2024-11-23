<template>

<section>
    <h3>
        <span>
            Mis Paneles > {{ name }}
        </span>
    </h3>
    <input 
        type="text"
        placeholder="Añade una lista"
        v-model="listName"
        @keyup.enter="add()"
    />

    <div class="container">
        <column
            v-for="(list, index) in boardList"
            :key="index"
            :listId="list.id"
            :name="list.name"
        >
        
        </column>
    </div>
</section>

</template>

<script>
import Column from '@/components/Column'
const Board = {
    name: 'board',
    components: {Column},
    props: {
        name: String,
        id: String
    },

    data() {
        return {
            listName: '',
            boardList: [
                {
                    id: '1', name: 'Todo'
                },
                {
                    id: '2', name: 'Doing'
                }
            ]
        }
    },

    methods: {
        add() {
            this.boardList.push({ name: this.listName })
        }
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

    input {
        background-color: #607D8B;
        border: 0;
        border-radius: 3px;
        box-shadow: 0 0 0 0.5px rgba(49,49,93,.03),
        0 2px 5px 0 rgba(49,49,93,.1),
        0 1px 2px 0 rgba(0,0,0,.08);
        color: #f7fcff;
        font-size: 1.2rem;
        margin: 0rem;
        outline: 0;
        padding: 1rem;
        transition: all 600ms ease;
        
        &:active,
        &:focus {
            background-color: #FAFAFA;
        }
        
    }
    
    span {
        color: #546e7a;
    }
</style>