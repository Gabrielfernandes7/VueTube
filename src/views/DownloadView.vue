<script setup>
import ButtonDownload from '@/components/ButtonDownload.vue';
import InputLink from '@/components/InputLink.vue';

let url = document.getElementsByName('url');

function downloadMusic(url) {
  let urlDownload = 'https://convert2mp3s.com/api/single/mp3?url=' + url;

  console.log(urlDownload);
  /*https://www.youtube.com/watch?v=JlMbfAI1iZc*/
}
  
</script>


<template>
  <div class="download">
    <InputLink v-on:click="downloadMusic(url)" />
    <ButtonDownload />
    <iframe src="https://convert2mp3s.com/api/single/mp3?url=https://www.youtube.com/watch?v=JlMbfAI1iZc"
      scrolling="yes" style="border:yes"></iframe>
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
