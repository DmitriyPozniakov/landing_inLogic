<template>
<section class="form-section">
        <div class="top">
            <div class="article">
                <div class="text">
                    <h2 class="heading">Ready to scale your project to the next level? <span><img
                                src="../assets/images/star_lightGreen.svg" alt=""></span></h2>
                    <p class="description">Lets' take your project to new heights, reach out and see how we can
                        help
                        you.</p>
                </div>
                <div class="review">
                    <img src="../assets/images/person1.jpeg" alt="" class="person person-1">
                    <img src="../assets/images/person2.jpeg" alt="" class="person person-2">
                    <img src="../assets/images/stars.svg" alt="stars" class="stars">
                    <p class="review-text">Rated 4.9/5.0 on UpWork and LinkedIn</p>
                </div>
            </div>
            <div class="form-wrapper">
                <form>
                    <div class="form-description">
                        <h2 class="form-title">Describe your project</h2>
                        <p class="form-text">Describe your idea below. We will contact you as soon as possible.</p>
                    </div>
                    <div class="form-fields">
                        <label for="fullName">Full name</label>
                        <input type="name" class="fullName" placeholder="Your name">
                        <label for="email">Email addres</label>
                        <input type="email" class="email" placeholder="Your email">
                        <label for="">Describe a project</label>
                        <textarea rows="10" placeholder="Description"></textarea>
                    </div>
                    <base-button text="Contact us" class="action-button">
                        Contact us
                        <img src="../assets/images/arrow.svg" alt="">
                    </base-button>
                </form>
            </div>
        </div>
    </section>
</template>

<script>
import BaseButton from './BaseButton.vue';
export default {
    components: { BaseButton }
}
</script>

<style scoped>
.form-section {
    background: #171e17;
    padding: 120px 60px;
    overflow:hidden;
}

.top {
    display: flex;
    justify-content: space-evenly;
    gap: 85px;
}

.article {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

.text {
    display: flex;
    flex-direction: column;
    gap: 30px;
}

.review {
    display: flex;
    align-items: center;
    /* gap: 20px */
}

.review-text {
    font-family: 'Gilroy-300';
    font-size: 16px;
    color: #D8DADF
}

.person {
    width: 60px;
    height: 60px;
    border-radius: 50%;
    object-fit: cover;
    flex-shrink: 0;
}

.person-2 {
    margin-left: -15px;
    outline: 5px solid #171e17;
    margin-right: 16px;
}

.stars {
    margin-right: 20px;
}

.form-wrapper {
    position: relative;
    width: 500px;
    min-height: 660px;
    z-index: 1;
    overflow: visible;
}

.form-wrapper::before {
    content: '';
    position: absolute;
    top: -105px;
    left: -350px;
    right: -350px;
    bottom: -50px;
    z-index: -1;
    background-image: url('../assets/images/element_portfolio.svg');
    background-size: cover;  
    background-position: center; 
    background-repeat: no-repeat;
    background-size: 90%;
    padding: 80px 0px;
    height: 100%;
}

form {
    padding: 40px 20px;
    display: flex;
    flex-direction: column;
    gap: 35px;
    background: #232c1e;
    border-radius: 28px;
    z-index: 10;
    box-shadow: -6px 4px 80px 7px rgba(210, 238, 96, 0.20);
    overflow: visible
}

.action-button {
    align-self: center;
}

input,
textarea {
    padding: 20px 12px;
    border-radius: 12px;
    background: #313d2a;
    border: none;
    outline: none;
    color: #fff;
    font-size: 16px;
    font-family: 'Gilroy-300';
    transition: 0.2s ease;

}

input:focus,
textarea:focus {
    outline: 1px solid #cfff65;
}

input:hover,
textarea:hover {
    background-color: #4B5944;
    cursor: pointer;
}

textarea {
    height: 150px;
    resize: none;
}

input::placeholder,
textarea::placeholder {
    font-family: 'Gilroy-300';
    font-size: 16px;
    color: #686E64;
}

.form-description {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    gap: 12px;
}

.form-text {
    max-width: 315px;
    font-family: 'Gilroy-300';
    font-size: 16px;
    color: #d3d3d3;
    text-align: center;
}

.form-title {
    font-family: 'Gilroy-600';
    font-size: 32px;
    color: #fff;
}

.heading {
    font-family: 'Gilroy-600';
    color: #fff;
    font-size: 68px;
    max-width: 650px;
}

.description {
    font-family: 'Gilroy-300';
    color: #e0e0e0;
    font-size: 16px;
}

.form-fields {
    display: flex;
    flex-direction: column;
    gap: 16px;
}

label {
    font-family: 'Gilroy-500';
    color: #fff;
    font-size: 16px;
}
</style>