<template>
    <div>
        <h2>Product {{ id }}</h2>
        <p>Product Details for product {{ id }}</p>
    </div>
</template>

<script setup>
    const { id } = useRoute().params;
</script>

<style scoped>

</style>