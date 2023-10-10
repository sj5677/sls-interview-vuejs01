<script setup>
import TheInstructionItem from './TheInstructionItem.vue'
</script>

<template>
  <TheInstructionItem>
    <template #icon>
      <ui-icon size="24">checklist</ui-icon>
    </template>
    <template #heading>Complete Button</template>
    Implement the Todo Item complete button to strike through the item when the Todo Item is marked as completed. You can add 'done' css class to 'todolist-item' using 
    <a href="https://vuejs.org/guide/essentials/class-and-style.html#binding-html-classes" target="_blank" rel="noopener">Class and Style Bindings</a>
  </TheInstructionItem>

  <TheInstructionItem>
    <template #icon>
      <ui-icon size="24">delete</ui-icon>
    </template>
    <template #heading>Remove item from Todo List</template>
    Using <a href="https://vuejs.org/guide/essentials/event-handling.html#event-handling" target="_blank" rel="noopener">Event Handlings</a>, implement the Todo Item delete button to ensure that the item is removed from the list when it's deleted. The icon button is implemented using 
    <a href="https://material.balmjs.com/actions/icon-button" target="_blank" rel="noopener">BalmUI icon button</a>
  </TheInstructionItem>

  <TheInstructionItem>
    <template #icon>
      <ui-icon size="24">toggle_on</ui-icon>
    </template>
    <template #heading>Sorting</template>
    <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort" target="_blank" rel="noopener">Sorts</a> the completed Todo Item to the bottom of the <a href="https://vuejs.org/guide/essentials/list.html#list-rendering" target="_blank" rel="noopener">lists</a>.
  </TheInstructionItem>

  <TheInstructionItem>
    <template #icon>
      <ui-icon size="24">info</ui-icon>
    </template>
    <template #heading>Empty List Message</template>
    Using <a href="https://vuejs.org/guide/essentials/conditional.html" target="_blank" rel="noopener">conditional rendering</a>. Add logic to display a message indicating that the list is empty when it doesn't contain any items.
  </TheInstructionItem>

  <TheInstructionItem>
    <template #icon>
      <ui-icon size="24">send</ui-icon>
    </template>
    <template #heading>Fix the form</template>
    Fix the Todo Item creation so that Todo Item can be added to the list
  </TheInstructionItem>
</template>
