<template>
    <main>
        <div class="container mb-5">
            <ToggleButton texto="Ver Seccion" @toggle="mostrar = !mostrar" />
            <ToggleSection 
                v-if="mostrar"
            />

        </div>
        <section class="container my-5">
            <h2 class="text-center my-5 display-5 fw-normal">{{ subtitulo }}</h2>
            <div class="row gap-5 justify-content-evenly" id="cards">
                <!-- Aqui deberian ir las tarjetas -->

                <div class="col-10 col-sm-10 col-md-5 col-lg-3"
                    v-for="card in cards"
                    :key="card.id"
                >
                <Card
                    :imagen="card.imagen"
                    :titulo="card.titulo"
                    :descripcion="card.descripcion"
                    />

                </div>
            </div>
        </section>
        <Opinions />
        <Payment />
    </main>
</template>
<script setup>
    import { ref } from 'vue';
    import Payment from './Payment.vue';
    import Opinions from './Opinions.vue'
    import Card from './Card.vue';

    const subtitulo = ref('Nuestros Platos')

    //Importar imagenes, repetir con cada plato
    import entrecot from '@/assets/img/entrecot.webp'

import ToggleButton from './ToggleButton.vue';
import ToggleSection from './ToggleSection.vue';

    //datos duros
    const cards = ref([ 
        {
            id: 1,
            titulo: "Entrecot",
            descripcion: "Carne bonita y rica",
            imagen: entrecot
        },
        {
            id: 2,
            titulo: "Entrecot",
            descripcion: "Carne bonita y rica",
            imagen: entrecot
        },
        {
            id: 3,
            titulo: "Entrecot",
            descripcion: "Carne bonita y rica",
            imagen: entrecot
        },
        {
            id: 4,
            titulo: "Entrecot",
            descripcion: "Carne bonita y rica",
            imagen: entrecot
        },
        {
            id: 5,
            titulo: "Entrecot",
            descripcion: "Carne bonita y rica",
            imagen: entrecot
        },
        {
            id: 6,
            titulo: "Entrecot",
            descripcion: "Carne bonita y rica",
            imagen: entrecot
        }
    ])

    const mostrar = ref(false)
</script>
<style scoped></style>