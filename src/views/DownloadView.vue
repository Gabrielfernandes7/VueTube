<script setup>
  import ButtonDownload from '@/components/ButtonDownload.vue';
  import InputLink from '@/components/InputLink.vue';
</script>


<template>
  <div class="download">
    <h1>Esta é a página do download</h1>
    <InputLink /> <ButtonDownload />
  </div>
</template>

<style>
  input .url{
    background-color: #0f9058;
    margin: 2rem;
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
