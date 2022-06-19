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
    <p> Sua url:{{ text }}</p>
    <a href="https://convert2mp3s.com/api/single/mp3?url=" id="link-download">
        <button @click="printar"> Download </button>
    </a>
</template>

<style>
a {
    text-decoration: none;
}

button, input{
    width: 15rem;
    height: 2.5rem;
    background-color: rgba(10, 241, 164, 0.219);
}

button:hover {
    background-color: aliceblue;
    color:black;
    font-family: 'Courier New', Courier, monospace;
}
</style>