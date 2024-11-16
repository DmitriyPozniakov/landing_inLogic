<template>
    <section class="our-services">
        <base-preheading text="Our services" backgroundColor="#E9F6E9" textColor="#000"></base-preheading>
        <h2 class="services-heading">What <span class="special-text">we offer</span></h2>
        <div class="offer-list">
            <div v-for="(offer, index) in offers" :key="index" class="offer-list-item">
                <img :src="offer.image" alt="" class="offer-image">
                <h2 class="offer-heading">{{ offer.title }}</h2>
                <p class="offer-description">{{ offer.description }}</p>
            </div>
        </div>
    </section>
</template>

<script>
import BasePreheading from './BasePreheading.vue';
export default {
    components: { BasePreheading },
    data() {
        return {
            offers: [
                {
                    image: require('@/assets/images/consulting.svg'),
                    title: 'IT Consulting',
                    description: 'Help organisations to streamline their operations, enhance communication, optimise performance, gain a competitive edge, and achieve their business goals.',
                },
                {
                    image: require('@/assets/images/mobile.svg'),
                    title: 'Mobile Development',
                    description: 'Developing innovative mobile apps for businesses and startups. We offer services such as optimization, redesign and other related tasks to provide our clients with comprehensive support.',
                },
                {
                    image: require('@/assets/images/softwareSettings.svg'),
                    title: 'Software Product Discovery',
                    description: 'Conducting research before the development process begins is crucial.',
                },
            ]
        }
    }
}
</script>

<style scoped>
.our-services {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 25px;
    padding: 90px 40px 40px 40px;
}

.services-heading {
    font-family: 'Gilroy-600';
    font-size: 68px;
    margin-bottom: 40px;
    position: relative;
}

.services-heading::after {
    content: '';
    position: absolute;
    top: -20px;
    right: -70px;
    background-image: url('../assets/images/greenStar.svg');
    background-size: cover;
    width: 55px;
    height: 55px;
}

.offer-list {
    display: flex;
    justify-content: center;
    border: 1px solid rgba(0, 0, 0, 0.05);
    border-radius: 20px;
    margin-bottom: 220px;
    position: relative;
}

.offer-list::before {
    content: '';
    position: absolute;
    background-image: url('../assets/images/blob\ 1.svg');
    background-repeat: no-repeat;
    height: 275px;
    inset: -150px 0 0 -145px;
    z-index: -1;
}

.offer-list::after {
    content: '';
    position: absolute;
    background-image: url('../assets/images/blob\ 2.svg');
    background-repeat: no-repeat;
    height: 150px;
    width: 300px;
    z-index: -1;
    inset: 180px -50px 0 995px;
}

.offer-list-item {
    max-width: 345px;
    padding: 28px 20px;
    background: transparent;
    background: #fff;
}

.offer-list-item:nth-child(odd) {
    border-radius: 20px;
}

.offer-list-item:nth-child(2) {
    border-left: 1px solid rgba(0, 0, 0, 0.05);
    border-right: 1px solid rgba(0, 0, 0, 0.05);
}

.offer-image {
    margin-bottom: 30px;
    height: 24px;
}

.offer-heading {
    font-family: 'Gilroy-600';
    color: #1B660D;
    font-size: 31px;
    margin-bottom: 9px;
}

.offer-description {
    font-family: 'Gilroy-300';
    color: #434343;
    font-size: 16px;
}
</style>