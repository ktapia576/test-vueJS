<template>
    <p>{{ greeting }}</p>
    <ol id=todoList>
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
                { id: 0, text: 'Vegetables' },
                { id: 1, text: 'Cheese' },
                { id: 2, text: 'Whatever else humans are supposed to eat' }
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