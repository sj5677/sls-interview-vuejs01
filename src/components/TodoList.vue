<script setup>
import TodoListItemCreate from './TodoListItemCreate.vue'
</script>

<template>
    <h1>Todo List</h1>
    <h5>Get things done, one item at a time.</h5>
    <div class="todolist-container">
        <ul  class="todolist">
            <li class="todolist-item" v-for="(item, index) in list">
                <span class="label">{{ item.title }}</span>
                <div class="actions">
                    <ui-icon-button v-model="item.done" :toggle="checkboxIcon"> </ui-icon-button>
                    <ui-icon-button icon="delete" @click="deleteTodoItem(item.id)"> </ui-icon-button>
                </div>
            </li>
        </ul>
        <p class="todolist-empty">The list is empty. Please add some Todo items.</p>
    </div>
    <TodoListItemCreate @add-item="addTodoItem" />
</template>

<script>
const checkboxIcon = {
    on: 'check_box',
    off: 'check_box_outline_blank'
};

export default {
    data() {
        return {
            checkboxIcon,
            list: [
                {
                    id: 1, title: 'Practice VueJs', done: false
                },
                {
                    id: 2, title: 'Talk to Jeremy', done: true
                },
                {
                    id: 3, title: `Grab some Pizza`, done: false
                },
                {
                    id: 4, title: `Buy a coffee`, done: true
                },
                {
                    id: 5, title: `Hangout with friends`, done: false
                }
            ]
        };
    },
    methods: {
        deleteTodoItem(id) {
            // TODO
        },
        addTodoItem(title) {
            this.list.push({
                id: Math.floor(Math.random() * 999999999), 
                title: title, 
                done: false
            });
        }
    }
};
</script>