<template>
        <button class="btn btn-primary" @click="$emit('toggle')">
            {{ texto }}
        </button>
</template>

<script setup>
    defineProps({
        texto: {
            type: String,
            default: 'Mostrar / Ocultar'
        }
    })
</script>