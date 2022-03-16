<template>
    <div class="contador">
        <h2>Contador : {{ contador }}</h2>
        <button @click="diminuirUm">-</button>
        <button @click="somarUm">+</button>
    </div>
</template>

<script>
export default {
    name: 'MeuContador',
    data() {
        return {
            contador: 0
        }
    },
    methods: {
        diminuirUm() {
            this.contador--;
        },
        somarUm() {
            this.contador++;
        }
    }
}
</script>

<style scoped>
    h2 {
        font-weight: bold;
    }
</style>