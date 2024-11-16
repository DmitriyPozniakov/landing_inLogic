<template>
    <section class="choose-us-section">
        <div class="choose-us-heading">
            <base-preheading text="Why work with us"></base-preheading>
            <h2 class="heading">Why inLogicSoft?</h2>
        </div>
        <p class="article">
            As a full-cycle development agency, we specialise in creating exceptional web and mobile applications
            for
            innovative businesses. Our team comprises specialists with diverse expertise across various industries.
        </p>
    </section>
    <div class="numeric">
        <div class="numeric-item">
            <strong>100+</strong>
            <p>Projects delivered</p>
        </div>
        <div class="numeric-item">
            <strong>4+</strong>
            <p>Years of experience</p>
        </div>
        <div class="numeric-item">
            <strong>2K+</strong>
            <p>Cups of coffee</p>
        </div>
    </div>
</template>

<script>
import BasePreheading from './BasePreheading.vue';
export default {
    components: { BasePreheading }
}
</script>

<style scoped>
.choose-us-section {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0px 40px;
    padding-bottom: 150px;
}

.choose-us-heading {
    display: flex;
    flex-direction: column;
    gap: 30px;
    align-items: flex-start;
}

.heading {
    font-family: 'Gilroy-600';
    font-size: 68px;
    color: #fff;
}

.article {
    font-family: 'Gilroy-300';
    font-size: 16px;
    color: #fff;
    max-width: 465px;
}

.numeric {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 170px;
    text-align: center;
    margin-bottom: 70px;
}

.numeric-item strong {
    color: #fff;
    font-family: 'Gilroy-600';
    font-size: 120px;    
}

.numeric-item p {
    color: #dbdbdb;
    font-family: 'Gilroy-300';
    font-size: 24px;
}
</style>