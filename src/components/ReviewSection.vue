<template>
    <section class="review-section">
        <div class="review-top">
            <base-preheading text="Reviews" backgroundColor="#e9f6e9" textColor="#000"></base-preheading>
            <h2 class="review-heading">Customers say <span class="special-text">about us</span></h2>
        </div>
        <div class="reviews">
            <div v-for="(review, index) in reviews" :key="index" class="review-item">
                <p class="review-company"><strong>{{ review.company }}</strong></p>
                <p class="review-description"> {{ review.description }}</p>
                <div>
                    <p class="review-person"> {{ review.person }}</p>
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
            reviews: [
                {
                    company: '‍Hapday LTD',
                    description: 'It was a wonderful iOS developers team. They are extremely calm and result-oriented. I suppose a combination of these two options is a key to successful development process.',
                    person: 'Gary R.',
                    mark: 4.9
                },
                {
                    company: 'NDA, Crypto Wallet',
                    description: 'Team performed extremely complicated tasks according to the deadlines we had.Communication and technical skills are on AAA level.',
                    person: 'James-Rodger K.',
                    mark: 5
                },
                {
                    company: 'VIO LTD',
                    description: 'The collaboration was excellent, and they displayed a high level of expertise in mobile app development, with an amazing attention to detail.',
                    person: 'Kiril J.',
                    mark: 4.9
                },
            ],
        }
    },
    methods: {
        // amountOfStars(mark) {
        //     const stars = Math.round(mark); 
        // }
    }
}
</script>

<style scoped>
.review-section {
    padding: 90px 40px 40px 40px;
}

.review-top {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 30px;
}

.review-heading {
    font-family: 'Gilroy-600';
    font-size: 68px;
    color: #000;
    position: relative;
    margin-bottom: 65px;
}

.review-heading::after {
    content: '';
    position: absolute;
    top: -20px;
    right: -70px;
    background-image: url('../assets/images/greenStar.svg');
    background-size: cover;
    width: 55px;
    height: 55px;
}

.reviews {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 30px;
    position: relative;
    margin-bottom: 150px;
}

.reviews::before {
    content: '';
    position: absolute;
    background-image: url('../assets/images/blob\ 2.svg');
    background-repeat: no-repeat;
    height: 150px;
    inset: 170px 0 0 40px;
    z-index: -1;
}


.review-item {
    padding: 30px 35px 20px 35px;
    border: 1px solid rgba(0, 0, 0, 0.05);
    border-radius: 20px;
    max-width: 520px;
    background-color: #fff;
}

.review-company {
    font-family: 'Gilroy-300';
    font-size: 16px;
    margin-bottom: 20px;
}

.review-description {
    font-family: 'Gilroy-300';
    font-size: 16px;
    margin-bottom: 45px;
}

.review-person {
    font-family: 'Gilroy-600';
    font-size: 22px;
}
</style>