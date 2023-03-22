<template>
    <div>
        <h1>Estoy en el articulo numero.{{ myid }}</h1>
    </div>
</template>
<script setup>
const route = useRoute()
const myid = ref(route.params.id);
</script>
