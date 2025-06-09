<template>
    <section class="advantages-section">
        <base-preheading text="Advantages"></base-preheading>
        <h2 class="advantages-title">We <span class="advantages-special">value your time</span> as much as we value our
            own</h2>
        <div class="advantages-table">
            <div v-for="(advantage, index) in advantages" :key="index" class="advantage-item">
                <img :src="advantage.image" alt="">
                <p class="advantage-description">{{ advantage.description }}</p>
            </div>
        </div>
    </section>
</template>

<script>
import BasePreheading from './base/BasePreheading.vue';
export default {
    components: { BasePreheading },
    data() {
        return {
            advantages: [
                {
                    image: require('@/assets/images/starAdv.svg'),
                    description: 'Get 100% transparency for the terms of your projects. Our process includes a thorough estimation of the scope of work, ensuring that we offer an honest quote for our services.',
                },
                {
                    image: require('@/assets/images/Moon.svg'),
                    description: 'We handle all unexpected situations with a great deal of care. We inform you about force majeure events, so you can make the best decision.',
                },
                {
                    image: require('@/assets/images/flower.svg'),
                    description: 'Our goal is to transform your ideas into reality. You can trust us to deliver as we are experts in our field.',
                }
            ]
        }
    }
}
</script>

<style scoped>
.advantages-section {
    padding: 190px 0 20px 80px;
    background: #171e17;
    background-image: url('../assets/images/circle.png');
    background-repeat: no-repeat;
    background-position: center ;
    
    background-position: calc(50% + 900px) calc(50% - 15%);

    background-size: 1800px;
}

.advantages-title {
    font-family: 'Gilroy-600';
    color: #fff;
    font-size: 6.8rem;
    max-width: 885px;
    margin-top: 65px;
    margin-bottom: 110px;
}

.advantages-special {
    color: #000;
    background-color: #cfff65;
}

.advantage-item {
    display: flex;
    flex-direction: column;
    align-items: start;
    gap: 35px;
    max-width: 350px;
}

.advantage-description {
    font-family: 'Gilroy-300';
    font-size: 1.6rem;
    color: #fff;
}

.advantages-table {
    display: flex;
    gap: 55px;
    margin-bottom: 140px;
}
</style>