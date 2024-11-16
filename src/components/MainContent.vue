<template>
    <main>
        <our-services></our-services>
        <our-portfolio></our-portfolio>
        <our-advantages></our-advantages>
        <review-section></review-section>
    </main>
</template>

<script>
import OurServices from './OurServices.vue';
import OurPortfolio from './OurPortfolio.vue';
import OurAdvantages from './OurAdvantages.vue';
import ReviewSection from './ReviewSection.vue';
export default {
    components: {OurServices, OurPortfolio, OurAdvantages, ReviewSection}
}

</script>