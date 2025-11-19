<script setup>
    import { ref } from 'vue';

    const copyright = ref('&copy; ' + new Date().getFullYear());
</script>

<template>
    <footer>
        <p>Copyright {{ copyright }}</p>
    </footer>
</template>

<style scoped>
    footer p {
        position: fixed;
        bottom: 0;
        padding-bottom: 20px;
        color: rgba(57, 46, 221, 0.548)
    }
</style>