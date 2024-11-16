<template>
    <section>
        <div class="wrapper">
            <base-preheading text="We are quality"></base-preheading>
            <div class="hero-text">
                <h1 class="hero-heading">Convert <span class="special-text">your idea</span> into reality now</h1>
                <p class="hero-paragraph">We are a team of professionals who provide High-quality services, and help our
                    customers grow their
                    businesses or create an MVP quickly.</p>
            </div>
            <div class="hero-buttons">
                <base-button>
                    Get a free quote
                </base-button>
                <button class="button-portfolio">
                    Our portfolio
                    <img src="../assets/images/arrowWhite.svg" alt="" class="arrow">
                </button>
            </div>
            <div class="scroll">
                <img src="../assets/images/scroll.svg" alt="scroll">
            </div>
        </div>
    </section>
</template>

<script>
import BaseButton from './BaseButton.vue';
import BasePreheading from './BasePreheading.vue';
export default {
    components: { BaseButton, BasePreheading }
}
</script>

<style scoped>
.wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 40px;
}

.arrow {
    height: 16px;
}

.hero-heading,
.hero-paragraph {
    color: #fff
}

.hero-text {
    display: flex;
    flex-direction: column;
    align-items: center;
    position: relative;
}

.hero-text::after {
    content: '';
    position: absolute;
    top: -10px;
    right: -40px;
    background-image: url('../assets/images/star.svg');
    background-size: cover;
    background-position: center;
    width: 55px;
    height: 55px;
}

.hero-heading {
    font-family: 'Gilroy-600';
    font-size: 82px;
    line-height: 90px;
    max-width: 750px;
    text-align: center;
    margin-bottom: 15px;
}

.hero-paragraph {
    font-family: 'Gilroy-300';
    font-size: 16px;
    color: #d1d1d1;
    max-width: 425px;
    text-align: center;
    margin-bottom: 25px;
}

.hero-buttons {
    display: flex;
    gap: 20px;
    margin-bottom: 60px;
}

.button-portfolio {
    padding: 16px 28px;
    border-radius: 28px;
    background: transparent;
    border: none;
    color: #fff;
    font-family: 'Gilroy-300';
    display: flex;
    gap: 15px;
}

.button-portfolio img {
    color: #fff;
}

.scroll {
    display: flex;
    justify-content: center;
    margin-bottom: 230px;
}
</style>