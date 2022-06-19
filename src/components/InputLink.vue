<script>
export default {
    data() {
        return {
            text: '',
        }
    },

    methods: {
        printar() {
            document.getElementById('link-download').href = `https://convert2mp3s.com/api/single/mp3?url=${this.text}`;
        }
    }
}
</script>

<template>
    <input v-model="text" placeholder="Edite" />
    <p> sua url:{{ text }}</p>
    <a href="https://convert2mp3s.com/api/single/mp3?url=" id="link-download">
        <button @click="printar"> Download </button>
    </a>
</template>

<style>
a {
    text-decoration: none;
}
</style>