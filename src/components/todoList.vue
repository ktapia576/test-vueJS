<template>
    <p>{{ greeting }}</p>
    <ol id="todoList">
        <li v-for="todo in todos">
        {{ todo.text }}
        </li>
    </ol>
</template>

<script>

export default {
    props: {
        greeting: String,
    },
    data() {
        return {
            todos: [
                { id: 0, text: 'Take car to mechanic' },
                { id: 1, text: 'Buy groceries' },
                { id: 2, text: 'Take pet out for a walk' }
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
}

a {
  color: #42b983;
}
</style>