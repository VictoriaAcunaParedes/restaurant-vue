<template>
    <section class="opinions" :style="{ backgroundImage: `url(${opinionsBg})`}">
        <h2 class="text-center mb-5">Nuestros Clientes Opinan</h2>

        <div id="carouselExample" class="carousel slide">
            <div class="carousel-inner">
                <div class="carousel-item active">
                    <div class="d-flex flex-column align-items-center">
                        <p class="fs-4 fst-italic text-center w-75">"Excelente atención, comida con temperatura
                            perfecta."</p>
                        <h5 class="fw-bold mt-3">– Judy Roa</h5>
                    </div>
                </div>
                <div class="carousel-item">
                    <div class="d-flex flex-column align-items-center">
                        <p class="fs-4 fst-italic text-center w-75">"Buenismo servicio, la comida me transporto a mi
                            ciudad natal"</p>
                        <h5 class="fw-bold mt-3">– Sergio Bellini</h5>
                    </div>
                </div>
                <div class="carousel-item">
                    <div class="d-flex flex-column align-items-center">
                        <p class="fs-4 fst-italic text-center w-75">"Celebramos nuestro aniversario, cada detalle hizo
                            magica la velada."</p>
                        <h5 class="fw-bold mt-3">– Victoria Reyes</h5>
                    </div>
                </div>
                <div class="carousel-item">
                    <div class="d-flex flex-column align-items-center">
                        <p class="fs-4 fst-italic text-center w-75">"Muy buena atencion, y platos deliciosos! Volveria
                            mil veces."</p>
                        <h5 class="fw-bold mt-3">– Rafaela Ortega</h5>
                    </div>
                </div>
                <div class="carousel-item">
                    <div class="d-flex flex-column align-items-center">
                        <p class="fs-4 fst-italic text-center w-75">"Ambiente agradable, la mejor experiencia culinaria
                            de la ciudad."</p>
                        <h5 class="fw-bold mt-3">– Cesar San Martin</h5>
                    </div>
                </div>
            </div>
            <button class="carousel-control-prev" type="button" data-bs-target="#carouselExample" data-bs-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Previous</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#carouselExample" data-bs-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Next</span>
            </button>
        </div>
    </section>
</template>

<script setup>
import opinionsBg from '../assets/img/opinios-wall.jpg'
</script>

<style scoped>
.opinions {
    background-size: cover;
    background-position: center;
    padding: 100px;
}

</style>