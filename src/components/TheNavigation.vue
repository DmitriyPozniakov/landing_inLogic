<template>
    <nav>
        <img src="../assets/images/Logo.svg" alt="logo">
        <ul class="nav-list">
            <li class="nav-item"><a href="#" class="nav-link">Services</a></li>
            <li class="nav-item"><a href="#" class="nav-link">Portfolio</a></li>
            <li class="nav-item"><a href="#" class="nav-link">About</a></li>
            <li class="nav-item"><a href="#" class="nav-link">Career</a></li>
        </ul>
        <base-button text="Contact us">
            Contact us
            <img src="../assets/images/arrow.svg" alt="">
        </base-button>
    </nav>
</template>

<script>
import BaseButton from './BaseButton.vue';
export default {
    components: { BaseButton }
}
</script>

<style scoped>
nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 150px;
}

.nav-list {
    display: flex;
    gap: 38px;
    list-style-type: none
}

.nav-link {
    text-decoration: none;
    color: #fff;
    font-size: 16px;
    font-family: 'Gilroy-300';
}
</style>