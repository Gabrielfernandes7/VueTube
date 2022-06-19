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
    <button @click="printar">
        <a href="https://convert2mp3s.com/api/single/mp3?url=" id="link-download">
            Download 
        </a>
    </button>
</template>