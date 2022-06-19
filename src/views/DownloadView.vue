<script setup>
import InputLink from '@/components/InputLink.vue';
</script>


<template>
  <div class="download">
    <p>
      <InputLink :value="text" />
    </p>
  </div>
</template>

<style>
  input .url{
    background-color: #0f9058;
    margin: 0.5rem;
    padding: 0.5rem;
  }

  button .botao-download{
    color: white;
    background-color: #0f9058;
  }

  @media (min-width: 1024px) {
    .download {
      min-height: 100vh;
      display: flex;
      align-items: center;
    }
  }
</style>
