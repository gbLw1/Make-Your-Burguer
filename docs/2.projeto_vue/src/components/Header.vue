<template>
    <div>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">Projetos</a></li>
            <li><a href="#">Contato</a></li>
        </ul>
    </div>
</template>


<script>

export default {
    name: 'Header'
}

</script>

<style scoped>

    ul {
        list-style: none;
        display: flex;
        background: #111;
    }

    li {
        margin-right: 10px;
    }

    a {
        color: #DDD;
        text-decoration: none;
        transform: .5s;
    }

    a:hover {
        color: turquoise;
    }

</style>