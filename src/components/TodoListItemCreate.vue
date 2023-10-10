<template>
    <form name="newform">
        <label for="newitem">Add to the Todo list</label>
        <input type="text" name="newitem" placeholder="e.g. eat an apple" v-model="title" />
        <button type="submit">Add item</button>
    </form>
</template>

<script>
export default {
    data() {
        return {
            title: "",
        };
    }
};
</script>