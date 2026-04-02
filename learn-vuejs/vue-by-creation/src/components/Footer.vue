<script setup>
    import { ref } from 'vue';

    const copyright = ref(new Date().getFullYear());
    const href = ref('https://vuejs.org');
</script>

<template>
    <footer>
        <!-- v-bind:href can be shortened to :href if the attribte has the same name as the variable-->
        Created using <a :href>Vue.js</a> &copy; {{ copyright}}
    </footer>
</template>

<style scoped>
footer {
    position:fixed;
    margin: 0 auto;
    bottom:0;
    text-align:center;
    color:#CCD6D9;
    padding-bottom:20px;
}

span{
    font-family: cursive;
}

a {
    color: white;
    text-decoration: none;
}
</style>