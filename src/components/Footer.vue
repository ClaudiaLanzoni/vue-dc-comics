<template>
    <footer>
        <div class="upper_footer_wrap">
            <div class="flex_list">
                <div>
                    <h2>Dc Comics</h2>
                    <ul>
                        <li v-for="(element, index) in listDCComics" :key="index">
                            <a :class={active:listDCComics.current} href="#">{{element.text}}</a>
                        </li>
                    </ul>

                    <h2>Shop</h2>
                    <ul>
                        <li v-for="(element, index) in listShop" :key="index">
                            <a :class={active:listShop.current} href="#">{{element.text}}</a>
                        </li>
                    </ul>
                </div>

                <div>
                    <h2>Dc</h2>
                    <ul>
                        <li v-for="(element, index) in listDC" :key="index">
                            <a :class={active:listDC.current} href="#">{{element.text}}</a>
                        </li>
                    </ul>
                </div>

                <div>
                    <h2>Sites</h2>
                    <ul>
                        <li v-for="(element, index) in listSites" :key="index">
                            <a :class={active:listSites.current} href="#">{{element.text}}</a>
                        </li>
                    </ul>
                </div>
            </div>
       
            <div class="overflow_bg">
                <img class="dc_logo_bg" src="../assets/vue-dc-comics-1/img/dc-logo-bg.png" alt="dc logo">
            </div>
        </div>

        <div class="downer_footer_wrap">

            <button class="btn_footer" >SIGN-UP NOW!</button>

            <div class="media_logo_section">
                <p class="my_inline">FOLLOW US</p>
                
                <img src="../assets/vue-dc-comics-1/img/footer-facebook.png" alt="Facebook logo">

                <img src="../assets/vue-dc-comics-1/img/footer-twitter.png" alt="Twitter logo">

                <img src="../assets/vue-dc-comics-1/img/footer-youtube.png" alt="Youtube logo">

                <img src="../assets/vue-dc-comics-1/img/footer-pinterest.png" alt="Pinterest logo">

                <img src="../assets/vue-dc-comics-1/img/footer-periscope.png" alt="Periscope logo">
            </div>

        </div>
    </footer>
</template>

<script>
export default {
    name : 'Footer',
    data : function () {
        return {
            index : 0,
            listDCComics : [
                {
                    text : "Characters",
                    url : "#",
                },
                {
                    text : "Comics",
                    url : "#",
                },
                {
                    text : "Movies",
                    url : "#",
                },
                {
                    text : "TV",
                    url : "#",
                },
                {
                    text : "Games",
                    url : "#",
                },
                {
                    text : "Videos",
                    url : "#",
                },
                {
                    text : "News",
                    url : "#",
                }],

            listShop : [
                {
                    text : "Shop DC",
                    url : "#",
                },
                {
                    text : "Shop DC Collectibles",
                    url : "#",
                }],

            listDC : [
                {
                    text : "Terms of use",
                    url : "#",
                },
                {
                    text : "Privacy policy (New)",
                    url : "#",
                },
                {
                    text : "Ad Choices",
                    url : "#",
                },
                {
                    text : "Advertising",
                    url : "#",
                },
                {
                    text : "Jobs",
                    url : "#",
                },
                {
                    text : "Subscriptions",
                    url : "#",
                },
                {
                    text : "Talent Workshops",
                    url : "#",
                },
                {
                    text : "CPSP Certificates",
                    url : "#",
                },
                {
                    text : "Ratings",
                    url : "#",
                },
                {
                    text : "Shop Help",
                    url : "#",
                },
                {
                    text : "Contact Us",
                    url : "#",
                }],

            listSites : [
                {
                    text : "DC",
                    url : "#",
                },
                {
                    text : "MAD Magazine",
                    url : "#",
                },
                {
                    text : "DC Kids",
                    url : "#",
                },
                {
                    text : "DC Universe",
                    url : "#",
                },
                {
                    text : "DC Power Visa",
                    url : "#",
                }
                ],



        }
    }
}
</script>

<style lang="scss" scoped>

@import "../style/variables.scss";
@import "../style/general.scss";

    ul {
        list-style: none;
        text-decoration-style: none;
        font-family: $listItemsFont;
        font-size: 10px;
      
    }

    li a {
        text-decoration: none;
        color: $whiteColor;
        line-height: 20px;
        word-spacing: 7px;
        

        &:hover {
            color : $dcLogoColor;
        }
    }

    .upper_footer_wrap {
        background-image: url('../assets/vue-dc-comics-1/img/footer-bg.jpg');
        height: 400px;
        display: flex;
        justify-content: space-between;
        padding: 0px 100px 0px 100px;
    }

    .downer_footer_wrap {
        display: flex;
        justify-content: space-between;
        background-color: $downerFooterBg;
        height: 80px;
        padding: 20px 100px 30px 100px;

        p {
            color: $dcLogoColor;
        }
    }

    .media_logo_section {

        img {
            padding-left: 15px;
        }
    }

    .my_inline {
        display: inline-block;
    }

    .flex_list {
        display: flex;
        justify-content: flex-start;
        
        div { 
            padding-right: 50px; 
            text-align: left;
        }

        h2 {
            color: $whiteColor;
            margin-bottom: 20px;
            padding-top: 40px;
        }
    }

    .overflow_bg {
        overflow: hidden;
    }

     .dc_logo_bg {
            height: 500px;
            width: 500px;
            margin-top: -35px;
        }


    .btn_footer {
      border-color: $dcLogoColor;
      color: $whiteColor;
      background-color: transparent;
      padding: 15px;
      text-align: center;
      text-decoration: none;
      display: inline-block;
      font-size: 15px;
      line-height: 4px;
      text-transform: uppercase;
      font-family: 'Staatliches';
    }
</style>