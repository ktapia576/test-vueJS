<template>
    <p>{{ greeting }}</p>
    <ul id="todoList">
        <li 
            @click="todo.complete = !todo.complete"
            v-bind:class="{ list: todo.complete}"
            v-for="todo in todos"
        >
        {{ todo.text }}
        </li>
    </ul>
</template>

<script>

export default {
    props: {
        greeting: String,
    },
    data() {
        return {
            todos: [
                { id: 0, text: 'Take car to mechanic', complete: false},
                { id: 1, text: 'Buy groceries', complete: false },
                { id: 2, text: 'Take pet out for a walk', complete: false }
            ]
        }
    }
}

</script>

<style scoped>
#todoList {
    margin: auto;
    width: 50%;
    border: 3px solid green;
    padding: 30px;
    text-align: left;
}

.list {
    text-decoration: line-through
}

a {
  color: #42b983;
}
</style>