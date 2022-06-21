<template>
    <div class="bg">
        <div class="container py-4 d-flex justify-content-between">
            <a href="#" class="sign-up">SIGN-UP NOW!</a>
            <div class="social d-flex gap-3 align-items-center">
                <a href="#" class="follow">FOLLOW US</a>
                <a href="#" class="social-icon"><img src="../assets/img/footer-facebook.png"></a>
                <a href="#" class="social-icon"><img src="../assets/img/footer-twitter.png"></a>
                <a href="#" class="social-icon"><img src="../assets/img/footer-youtube.png"></a>
                <a href="#" class="social-icon"><img src="../assets/img/footer-pinterest.png"></a>
                <a href="#" class="social-icon"><img src="../assets/img/footer-periscope.png"></a>
            </div>
        </div>
    </div>
</template>

<script>
    export default{

    }
</script>

<style lang="scss" scoped>
    .bg{
        background-color: #2f2f2f;
        position: fixed;
        bottom: 0;
        width: 100%;
    }

    .sign-up{
        padding: 0.5rem;
        border: 2px solid #3f7ef8;
        text-decoration: none;
        color: white;
    }

    .follow{
        color: #3f7ef8;
        text-decoration: none;
        font-weight: bold;
    }
</style>