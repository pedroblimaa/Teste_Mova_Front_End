<template>
  <button v-on:click="$emit('clicked')" class="btn">{{txt}}</button>
</template>

<script>
export default {
  name: "Button",
    props: ['txt']
};
</script>

<style scoped>
.btn {
    transition: 0.2s;
    cursor: pointer;
    padding: 10px 20px;
    border: 1px solid grey;
    border-radius: 3px;
    background-color: #1f1f1f;
    color: #fff;
}

.btn:hover {
    cursor: pointer;
    background-color: #111111
}

</style>
