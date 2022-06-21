<template>
    <header class="container d-flex justify-content-between align-items-center">
        <div class="brand py-4">
            <img alt="DC Logo" src="../assets/img/dc-logo.png">
        </div>
        <ul class="list-unstyled d-flex gap-3">
            <li v-for="(link, i) in navbarLinks" :key="i">
                <a :href="link.href" class="text-decoration-none text-uppercase fw-bold">
                {{ link.name }}
                <div class="hover-border"></div>
                </a>
            </li>
        </ul>
    </header>
</template>

<script>
    export default{
        data(){
            return{
                navbarLinks:[
                    {
                        name: "Characters",
                        href: "#"
                    },{
                        name: "Comics",
                        href: "#"
                    },{
                        name: "Movies",
                        href: "#"
                    },{
                        name: "Tv",
                        href: "#"
                    },{
                        name: "Games",
                        href: "#"
                    },{
                        name: "Collectibles",
                        href: "#"
                    },{
                        name: "Videos",
                        href: "#"
                    },{
                        name: "Fans",
                        href: "#"
                    },{
                        name: "News",
                        href: "#"
                    },{
                        name: "Shop",
                        href: "#"
                    },
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    header{
        .brand{
            $maxHeight: 70px;
            
            img{
                max-height: $maxHeight;
            }
        }

        ul{ margin-bottom: 0;
            li a{
            color: rgb(33,37,41);
            height: 100%;
            position: relative;

            &:hover{
                color: #3f7ef8;

                .hover-border{
                    display: block;
                }
            }

            .hover-border{
                width: 100%;
                height: 6px;
                position: absolute;
                bottom: -50px;
                left: 0;
                background-color: #3f7ef8;
                display: none;
            }
        }}
    }
</style>