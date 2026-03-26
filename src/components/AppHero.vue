<template>
    <header class="hero" :style="{ backgroundImage: `url(${heroBg})`}">
        <h1 class="text-center my-1 display-1 fw-medium">Restaurantcito</h1>
        <div class="text-center my-5">
            <!-- button trigger modal -->
            <button type="button" class="btn btn-warning btn-lg" data-bs-toggle="modal" data-bs-target="#exampleModal">
                Reserva tu mesa aqui
            </button>
            <!-- Modal -->
            <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel"
                aria-hidden="true">
                <div class="modal-dialog">
                    <div class="modal-content">
                        <div class="modal-header">
                            <h1 class="modal-title fs-5" id="exampleModalLabel">Bienvenido al Restaurantcito</h1>
                            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                        </div>
                        <div class="modal-body">
                            <form>
                                <label class="form-label">Nombre:</label>
                                <input class="form-control mb-2" type="text">
                                <label class="form-label">Numero de personas:</label>
                                <input class="form-control mb-2" type="number">
                                <label class="form-label">Fecha:</label>
                                <input class="form-control mb-3" type="date">
                                <button class="btn btn-primary w-100">Enviar Reserva</button>
                            </form>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>

<script setup>
    import { ref } from 'vue'
    import heroBg from '@/assets/img/background-image.jpg'
    import AppReservationModal from './AppReservationModal.vue';

    const mostrarModal = ref(false)


</script>

<style scoped>
.hero {
    background-size: cover;
    background-position: center;
    padding: 150px;
}

@media (max-width: 768px) {
    .hero {
        padding: 120px 40px;
    }
}

h1 {
    font-weight: 700;
}
</style>