<script setup>
    import { ref } from 'vue';

    const quote = ref('First, solve the problem. Then, write the code.');
    const author = ref('John Johnson');
    const href = ref('https://www.google.com');
    const isBtnDisabled = ref(true);

    quote.value = 'Interpolation is the process of replacing variables with their values in a string.';
    author.value = 'Professor Pickle';

</script>

<template>
    <main>
        <section>
            <p>{{ quote }}</p>
            <!-- v-bind:href can be shortened to :href if the attribte has the same name as the variable-->
            <span><a :href>{{ author }}</a></span>
        </section>
        <section id="buttons">
            <!-- v-bind:something can be shortened to :something-->
            <button :disabled="isBtnDisabled">Another!</button>
            <button v-bind:disabled="isBtnDisabled">Share!</button>
        </section>
    </main>
</template>

<style scoped>
main {
    background: #CCD6D9;
    max-width: 90%;
    border-radius: 0 15px 0 15px;
    padding: 35px;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 10px;
}

section {
    display: flex;
    width: 100%;
    flex-direction: column;
    gap: 10px;
    margin-bottom: 25px;
}

p {
    font-weight: bold;
    font-style: italic;
    font-size: 2rem;
    text-align: left;
}

p::before {
    content: '"'
}

p::after {
    content: '"'
}

span {
    align-self: end;
    color: #406473;
}

span::before {
    content: "- "
}

span a {
    color: #406473;
    text-decoration: none;
}

#buttons {
    display:grid;
    grid-template-columns: 2fr 1fr;
  }

  button {
      background:#406473;
      color: white;
      padding:10px;
      border: 0;
      font-size:1.2rem;
      border-radius:0 5px 0 5px;
      font-weight:bold;
      margin-top:20px;
      cursor:pointer;
      transition: transform 0.2s;
  }
  button:hover{
      transform: scale(1.05);
  }
  button:disabled {
  background:grey;
  cursor: not-allowed;
  opacity:0.5;
}
</style>