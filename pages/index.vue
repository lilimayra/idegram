<template>
    <div>
        <h1>Pagina Home</h1>
        <p>Texto de home</p>
        <p><nuxt-link to="/blog">ir al blog</nuxt-link></p>
        <h1>Usuarios</h1>
        <User v-for="user in users" :name="user.name" />
    </div>
</template>

<script setup>

    const { data: users } = await useFetch('https://jsonplaceholder.typicode.com/users')
</script>