<template>
    <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>

export default {
    name: 'LifeCycle',
    data() {
        return {
            nome: 'Ainda não sei'
        }
    },
    created() {
        setTimeout(() => {
            this.nome = 'Gabriel';
        }, 1000);

        this.lifeCycle()
    },
    mounted() {
        setTimeout(() => {
            this.nome = 'Lucas';
        }, 2000);

        this.lifeCycle()
    },
    methods: {
        lifeCycle() {
            console.log("Executou")
        }
    }
}

</script>