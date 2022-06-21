<template>
    <div class="section">
        <div class="container d-flex text-start gap-4 text-light py-4">
            <div>
                <h4>DC COMICS</h4>
                <ul class="list-unstyled">
                    <li v-for="link in comicsLinks" :key="link">{{ link }}</li>
                </ul>

                <h4>SHOP</h4>
                    <ul class="list-unstyled">
                    <li v-for="link in shopLinks" :key="link">{{ link }}</li>
                </ul>
            </div>
            <div>
                <h4>DC</h4>
                <ul class="list-unstyled">
                    <li v-for="link in DCLinks" :key="link">{{ link }}</li>
                </ul>
            </div>
            <div>
                <h4>SITES</h4>
                <ul class="list-unstyled">
                    <li v-for="link in sitesLinks" :key="link">{{ link }}</li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
    export default{
        data(){
            return{
                comicsLinks: [
                    "Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"
                ],
                shopLinks: [
                    "Shop DC", "Shop DC Collectibles"
                ],
                DCLinks: [
                    "Terms of use", "Privacy Policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us"
                ],
                sitesLinks: [
                    "DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    .section{
        background: url("../assets/img/footer-bg.jpg");
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        margin-bottom: 90px;
    }

    h4{
        font-weight: bold;
    }

    li{
        color: grey;
    }
</style>