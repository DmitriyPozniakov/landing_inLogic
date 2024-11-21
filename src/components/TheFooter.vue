<template>
    <footer>
        <div class="footer-figure">
            <div class="figure-top">
                <div class="figure-left-top">
                    <img src="../assets/images/Logo.svg" alt="">
                    <img src="../assets/images/comName.svg" alt="">
                </div>
                <div class="figure-right-top">
                    <img src="../assets/images/upWork.svg" alt="">
                    <img src="../assets/images/linkedIn.svg" alt="">
                </div>
            </div>
            <hr>
            <div class="figure-bottom">
                <div class="sections">
                    <ul class="list">
                        <li><a href="#">Services</a></li>
                        <li><a href="#">Portfolio</a></li>
                        <li><a href="#">About</a></li>
                        <li><a href="#">Career</a></li>
                    </ul>
                    <p class="our-location">We are based in <strong>Lviv</strong></p>
                </div>

            </div>
        </div>
        <p class="copyright">2024 &copy; Copyright inlogicsoft. All Rights Reserved</p>
    </footer>
</template>

<style scoped>
footer {
    padding: 60px 60px 30px 60px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background: #171e17;
    

}

.footer-figure {
    width: 100%;
    padding: 25px 50px;
    margin-bottom: 30px;
    border-radius: 25px;
    background: linear-gradient(80deg, rgba(35,44,30,1) 61%, rgba(189,238,96,0.804359243697479) 100%);


}

.figure-top {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 80px;
}

.figure-right-top {
    display: flex;
    gap: 4px;
}

hr {
    opacity: 0.1;
    margin-bottom: 30px;
}

.sections {
    display: flex;
    align-content: center;
    justify-content: space-between;
}

.list {
    display: flex;
    gap: 40px;
}

a,
.our-location {
    font-family: 'Gilroy-300';
    color: #fff;
    font-size: 16px;
}

.copyright {
    font-family: 'Gilroy-300';
    color: #fff;
    font-size: 16px;
}
</style>