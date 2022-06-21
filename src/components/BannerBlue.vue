<template>
    <div class="section">
        <div class="container">
            <ul class="d-flex py-4 list-unstyled justify-content-evenly align-items-center">
                <li>
                    <a href="#" class="text-decoration-none d-flex">
                        <img src="../assets/img/buy-comics-digital-comics.png">
                        <p>DIGITAL COMICS</p>
                    </a>
                </li>
                <li>
                    <a href="#" class="text-decoration-none d-flex">
                        <img src="../assets/img/buy-comics-merchandise.png">
                        <p>DC MERCHANDISE</p>
                    </a>
                </li>
                <li>
                    <a href="#" class="text-decoration-none d-flex">
                        <img src="../assets/img/buy-comics-subscriptions.png">
                        <p>SUBSCRIPTION</p>
                    </a>
                </li>
                <li>
                    <a href="#" class="text-decoration-none d-flex">
                        <img src="../assets/img/buy-comics-shop-locator.png">
                        <p>COMIC SHOP LOCATOR</p>
                    </a>
                </li>
                <li>
                    <a href="#" class="text-decoration-none d-flex">
                        <img src="../assets/img/buy-dc-power-visa.svg">
                        <p>DC POWER VISA</p>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default{
        
    }
</script>

<style lang="scss" scoped>
    .section{
        background-color: #3f7ef8;
        color: whitesmoke;

        .container ul{ margin-bottom: 0;
            li a{
            align-items: center;
            gap: 0.5rem;

            img{
                max-height: 70px;
                max-width: 60px;
                align-self: center;
            }

            p{
                white-space: nowrap;
                margin-bottom: 0;
            }

            &:hover{
                color: rgba(255,255,255,0.7);
            }
        }}
    }
</style>