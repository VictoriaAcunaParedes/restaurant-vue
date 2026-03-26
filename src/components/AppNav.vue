<template>
    <nav class="navbar navbar-expand-lg bg-azulito" data-bs-theme="dark">
        <div class="container">
            <a class="navbar-brand col-2" href="#"><img class="logo-chefcito" :src="logo"
                    alt="logo-chefcito"></a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup"
                aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
                <div class="navbar-nav ms-auto">
                    <a class="nav-link active fs-3" aria-current="page" href="#">{{ home }}</a>
                    <a class="nav-link fs-3" href="#">Nuestros Platos</a>
                    <a class="nav-link fs-3" href="#">Contacto</a>
                </div>
            </div>
        </div>
    </nav>
</template>

<script setup>
    import logo from '@/assets/img/chefcito.png'
    import { ref } from 'vue';

    const home = ref("Inicio")
</script>
    

<style scoped>
    .logo-chefcito {
        width: 30%;
    }
</style>