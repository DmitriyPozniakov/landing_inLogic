<template>
    <header>
        <the-navigation></the-navigation>
        <the-hero></the-hero>
        <choose-us></choose-us>
    </header>
</template>

<script>
import TheNavigation from './TheNavigation.vue';
import TheHero from './TheHero.vue';
import ChooseUs from './ChooseUs.vue';
export default {
    components: { TheNavigation, TheHero, ChooseUs }
}
</script>

<style scoped>
header {
    padding: 0 40px;
    background-color: #171e17;
    background-image: url('../assets/images/background.svg');
    background-repeat: no-repeat;
    background-size: 145%;
    background-position: 20% 120%;
    padding-bottom: 120px; 
}
</style>