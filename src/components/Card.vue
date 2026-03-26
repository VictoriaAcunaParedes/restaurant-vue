<template>
    <div class="card p-0">
        <img :src="imagen" class="card-img-top" :alt="titulo">
        <div class="card-body">
            <h5 class="card-title">{{titulo}}</h5>
            <p class="card-text">{{ descripcion }}</p>
            <button class="btn btn-primary" data-bs-toggle="popover" data-bs-title="Alergenos | Kcal" data-bs-content="Frutos secos - Sulfitos | 704 kcal">Detalle</button>
        </div>
    </div>
</template>

<script setup>
    defineProps({
        imagen: String,
        titulo: String,
        descripcion: String
    })
</script>
<style scoped></style>