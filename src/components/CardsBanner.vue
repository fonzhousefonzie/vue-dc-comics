<template>
    <div class="cards-sections-container">
        <div class="cards-jumbo" :style="{backgroundImage: 'url(' + url + ')'}">
            <div class="container">
                <h3>CURRENT SERIES</h3>
            </div>
        </div>
        <div class="cards-section">
            <div class="container">
                <div class="row">
                    <div class="col col-6 col-sm-4 col-md-2" v-for="(comic, i) in comics" :key="comic.series" @click="active(i)" :class="{active : comic.isActive}">
                        <ComicCard :img-url="comic.thumb" :cardTitle="comic.series"/>
                    </div>
                </div>
                <button class="primary">LOAD MORE</button>
            </div>
        </div>
    </div>
</template>

<script>
import ComicCard from './ComicCard.vue'


export default {
    data() {
        return {
            url : require("../assets/img/jumbotron.jpg"),
            comics: [
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book",
                    "isActive": false,
                    "jumbo": "https://cdn.wallpapersafari.com/71/44/SYh8Ww.jpg"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book",
                    "isActive": false,
                    "jumbo": "https://1.bp.blogspot.com/-g1KWx10F3P4/X3t1kTOHMsI/AAAAAAAA07c/GUnqYGnEVEgKmJPkdab5jCASyWHHMU5SgCLcBGAsYHQ/s1920/AMERICAN%2BVAMPIRE%2B1976%2B03%2B-%2BMAIN_5f73cc3eec5988.41001566.jpg"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel",
                    "isActive": false,
                    "jumbo": "https://images.alphacoders.com/237/237033.jpg"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book",
                    "isActive": false,
                    "jumbo": "https://wallpaper.dog/large/17203361.jpg"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book",
                    "isActive": false,
                    "jumbo": "https://thecomicvault.files.wordpress.com/2017/09/cover-bman.jpg"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book",
                    "isActive": false,
                    "jumbo": "https://www.blogo.it/app/uploads/sites/3/2021/08/the-batman-i-fumetti-che-hanno-ispirato-il-reboot-di-matt-reeves-5-copia.jpg"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book",
                    "isActive": false,
                    "jumbo": "https://images2.alphacoders.com/623/623846.jpg"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book",
                    "isActive": false,
                    "jumbo": "https://images4.alphacoders.com/103/1033031.jpg"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book",
                    "isActive": false,
                    "jumbo": "https://static1.srcdn.com/wordpress/wp-content/uploads/2020/06/Batman-Nightwing-Joker-War-Cover-Image.jpg?q=50&fit=crop&w=960&h=500&dpr=1.5"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book",
                    "isActive": false,
                    "jumbo": "https://images2.alphacoders.com/108/1086193.jpg"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book",
                    "isActive": false,
                    "jumbo": "https://1.bp.blogspot.com/-DnHd0QMjxNc/X44sDvlQZYI/AAAAAAAA1Gk/74UhtX5CynMrJAo_LDUP8jACr4I7W2vzgCLcBGAsYHQ/s1920/BWKP_HQ_Cv1_C2-C3V2_03_5f7e3c2dc1b153.85639803.jpg"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel",
                    "isActive": false,
                    "jumbo": "https://www.dccomics.com/sites/default/files/Gallery_20200408_Catwoman_%2322-cover_5e850ef3cf9258.40151769.jpg"
                }
            ]
        };
    },
    methods: {
        active(i) {
            let th = this;
            for (let j = 0; j < this.comics.length; j++){
            th.comics[j].isActive = false;
            }
            this.comics[i].isActive = true;
            this.url = th.comics[i].jumbo;
        }
    },
    components: { ComicCard }
}
</script>

<style lang="scss" scoped>
.cards-sections-container {
    background-color: #2f2f2f;

    .cards-jumbo {
        height: 300px;
        background-position: top center;
        background-repeat: no-repeat;
        background-size: cover;
        text-align: start;
        position: relative;

        h3 {
            display: inline-block;
            color: whitesmoke;
            font-weight: bold;
            padding: 1rem;
            background-color: #3f7ef8;
            position: absolute;
            bottom: 0;
            transform: translateY(50%);
            z-index: 10;
        }
    }

    .cards-section .container {
        padding: 1rem 0 2rem;

        .row {
            padding: 2rem;

            .col:hover{
                background: #3f7ef8;
            }
            .active{
                background: #3f7ef8;
            }
        }
    }
}
</style>