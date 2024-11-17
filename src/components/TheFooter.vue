<template>
    <footer>
        <div class="footer-top">
            <div class="footer-article">
                <h2 class="footer-heading">Ready to scale your project to the next level? <span><img src="../assets/images/star_lightGreen.svg" alt=""></span></h2>
                <p class="footer-description">Lets' take your project to new heights, reach out and see how we can help
                    you.</p>
            </div>
            <form>
                <div class="form-description">
                    <h2 class="form-title">Describe your project</h2>
                    <p class="form-text">Describe your idea below. We will contact you as soon as possible.</p>
                </div>
                <div class="form-fields">
                    <label for="fullName">Full name</label>
                    <input type="text" class="fullName" placeholder="Your name">
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
    </footer>
</template>

<script>
import BaseButton from './BaseButton.vue';
export default {
    components: { BaseButton }
}
</script>

<style scoped>
footer {
    background: #171e17;
    padding: 120px 60px;
}

.footer-top {
    display: flex;
    justify-content: space-evenly;
    gap: 85px;
}

.footer-article {
    display: flex;
    flex-direction: column;
    gap: 30px;
}

form {
    padding: 40px 20px;
    display: flex;
    flex-direction: column;
    gap: 35px;
    background-color: #232c1e;
    border-radius: 28px;
    box-shadow: -6px 4px 80px 7px rgba(210, 238, 96, 0.20);
    width: 500px;
    min-height: 660px;
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
    color: #686E64;
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

.footer-heading {
    font-family: 'Gilroy-600';
    color: #fff;
    font-size: 68px;
    max-width: 650px;
}

.footer-description {
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