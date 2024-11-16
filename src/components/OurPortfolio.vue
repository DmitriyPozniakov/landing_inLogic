<template>
    <section class="portfolio-section">
        <div class="wrapper">
            <div class="portfolio-top">
                <base-preheading text="Our portfolio"></base-preheading>
                <h2 class="portfolio-title">Cases we're pretty proud of</h2>
            </div>
            <div class="our-apps">
                <div v-for="(app, index) in apps" :key="index" class="app">
                    <div class="our-apps-text">
                        <div class="first-line">
                            <h2 class="app-title">{{ app.title }}</h2>
                            <p class="app-numeric">{{ app.numeric }}</p>
                        </div>
                        <div class="second-line">
                            <p class="app-description">{{ app.description }}</p>
                            <img src="../assets/images/arrowWhite.svg" alt="" class="arrow">
                        </div>
                    </div>
                    <img :src="app.image" alt="" class="app-image">
                </div>
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
            apps: [
                {
                    title: 'UMITY',
                    numeric: '01',
                    description: 'DESIGN + DEVELOPMENT',
                    image: require('@/assets/images/umity.png')
                },
                {
                    title: 'SPRT',
                    numeric: '02',
                    description: 'DESIGN + DEVELOPMENT',
                    image: require('@/assets/images/sprt.png')
                }
            ]
        }
    }
}
</script>

<style scoped>
.portfolio-section {
    padding: 150px 0 0 80px;
    background: #171e17;
    overflow: hidden;
    background-image: url('../assets/images/element_portfolio.svg');
    background-repeat: no-repeat;
    background-position: calc(50% + 900px) calc(50% - 65%);
    background-size: 900px;
}
.portfolio-top,
.first-line,
.second-line {
    display: flex;
    justify-content: space-between;
    align-items: start;
}

.our-apps {
    display: flex;
    gap: 35px;
    overflow: scroll;
}

.arrow {
    width: 33px;
    outline: #fff;
}

.app-image {
    width: 950px;
    height: 650px;
    border-radius: 30px;
    object-fit: cover;
    /* изображение масштабируется, заполняя контейнер */
    object-position: center;
    /* центрирование изображения */
}

.portfolio-title {
    font-family: 'Gilroy-600';
    font-size: 68px;
    color: #fff;
    width: 620px;
    margin-bottom: 150px;
    margin-right: 40px;
}

.app-title {
    font-family: 'Gilroy-600';
    font-size: 62px;
    color: #fff;
    margin-bottom: 15px;
}

.app-numeric {
    font-family: 'Gilroy-300';
    font-size: 16px;
    color: #fff;
}

.app-description {
    font-family: 'Gilroy-300';
    font-size: 22px;
    color: #fff;
    margin-bottom: 45px;
}
</style>
