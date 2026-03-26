<template>
    <section class="py-5 bg-azulito text-white d-none d-lg-block">
        <div class="container d-flex justify-content-between py-5">
            <h2 class="display-5 fw-medium">{{payment}}</h2>
            <div class="d-flex gap-4">
                <i class="fa-brands fa-cc-visa fa-4x"></i>
                <i class="fa-brands fa-cc-mastercard fa-4x"></i>
                <i class="fa-brands fa-cc-amex fa-4x"></i>
                <i class="fa-brands fa-cc-paypal fa-4x"></i>
                <i class="fa-brands fa-cc-diners-club fa-4x"></i>
                <i class="fa-brands fa-cc-discover fa-4x"></i>
            </div>
        </div>
    </section>
</template>

<script setup>
    import { ref } from 'vue';
    const payment = ref("Medios de Pago")
</script>

<style scoped></style>