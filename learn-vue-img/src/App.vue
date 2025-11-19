<script setup>
  import catmeme3_a from '@/assets/images/catmeme3_a.jpg';
  import catmeme3_b from '@/assets/images/catmeme3_b.jpg';
</script>

<template>
  <section>
    <!-- Absolute path to /public folder -->
     <img src="/images/catmeme1_a.jpg" alt="cat meme 1a">
     <img src="/images/catmeme1_b.jpg" alt="cat meme 1b">
  </section>

  <section>
    <!-- Relative path to /assets folder -->
     <img src="@/assets/images/catmeme2_a.jpg" alt="cat meme 2a">
     <img src="@/assets/images/catmeme2_b.jpg" alt="cat meme 2b">
  </section>
  
  <section>
    <!-- Import asset into component -->
     <img v-bind:src="catmeme3_a" alt="cat meme 3a">
     <img v-bind:src="catmeme3_b" alt="cat meme 3b">
  </section>
</template>

<style scoped>
  section {
    display:grid;
    grid-template-columns:1fr 1fr;
    padding:10px;
    background:white;
    border-radius:10px;
  }
  img{
    width:100%;
  }
</style>
