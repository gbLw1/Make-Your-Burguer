<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Estou em busca de novas oportunidades!</p>
        <p>Utilizo as seguintes tecnologias:</p>
        <ul>
            <li>JavaScript</li>
            <li>.NET C#</li>
            <li>Python</li>
        </ul>
        <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
        <p>Para acessar meu portfólio <a v-bind:href="link_portfolio" target="_blank">basta clicar aqui</a></p>
        <Picture />
    </div>
</template>

<script>

import Picture from './Picture.vue';

export default {
    name: 'Info',
    components: {
        Picture
    },
    data() {
        return {
            esta_trabalhando: true, 
            email: "gbl@mail.com",
            mostrar_email: true,
            link_portfolio: 'https://github.com/gbLw1'
        }
    }
}

</script>