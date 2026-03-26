<template>
        <footer class="bg-dark text-white py-5">
        <div class="container py-5">
            <div class="row justify-content-evenly justify-content-md-between">
                <div class="col-10 col-sm-10 col-md-6 mb-5 mb-md-0">
                    <h5 class="mb-5 fs-1">Contacto y Ubicación</h5>
                    <p><strong>{{ owner }}</strong></p>
                    <p><i class="fa-solid fa-phone"></i> +56911111111</p>
                    <p><i class="fa-solid fa-envelope"></i> alfredo.linguini@restaurantcito.cl</p>
                    <p><i class="fa-solid fa-location-dot"></i> Calle Falsa 123</p>
                </div>
                <div class="col-10 col-sm-10 col-md-6 mb-5 mb-md-0">
                    <h5 class="mb-5 fs-1">Desarrollado por Curso 0044</h5>
                    <div class="d-flex justify-content-evenly">
                        <p><i class="fa-brands fa-square-github fa-3x" data-bs-toggle="tooltip" data-bs-title="GitHub"></i></p>
                        <p><i class="fa-brands fa-linkedin fa-3x" data-bs-toggle="tooltip" data-bs-title="Linkedin"></i></p>
                        <p><i class="fa-brands fa-instagram fa-3x" data-bs-toggle="tooltip" data-bs-title="Instagram"></i></p>
                    </div>
                </div>
            </div>
        </div>
    </footer>

</template>

<script setup>
    import { ref } from 'vue';
    const owner = ref('Alfredo Linguini')
</script>

<style scoped></style>