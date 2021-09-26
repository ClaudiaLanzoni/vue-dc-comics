<template>
  <div>
        <h2>Dc Comics</h2>
        <ul>
            <li v-for="(element, index) in listDCComics" :key="index">
                <a :class={active:listDCComics.current} href="">{{element.text}}</a>
            </li>
        </ul>

        <h2>Shop</h2>
        <ul>
            <li v-for="(element, index) in listShop" :key="index">
                <a :class={active:listShop.current} href="">{{element.text}}</a>
            </li>
        </ul>

        <h2>Dc</h2>
        <ul>
            <li v-for="(element, index) in listDC" :key="index">
                <a :class={active:listDC.current} href="">{{element.text}}</a>
            </li>
        </ul>

        <h2>Sites</h2>
        <ul>
            <li v-for="(element, index) in listSites" :key="index">
                <a :class={active:listSites.current} href="">{{element.text}}</a>
            </li>
        </ul>


        <div>
            <button>SIGN-UP NOW!</button>

            <p>FOLLOW US</p>
            
            <img src="../assets/vue-dc-comics-1/img/footer-facebook.png" alt="Facebook logo">

            <img src="../assets/vue-dc-comics-1/img/footer-twitter.png" alt="Twitter logo">

            <img src="../assets/vue-dc-comics-1/img/footer-youtube.png" alt="Youtube logo">

            <img src="../assets/vue-dc-comics-1/img/footer-pinterest.png" alt="Pinterest logo">

            <img src="../assets/vue-dc-comics-1/img/footer-periscope.png" alt="Periscope logo">
        </div>
  </div>
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
                    current : false,
                },
                {
                    text : "Comics",
                    url : "#",
                    current : true,
                },
                {
                    text : "Movies",
                    url : "#",
                    current : false,
                },
                {
                    text : "TV",
                    url : "#",
                    current : false,
                },
                {
                    text : "Games",
                    url : "#",
                    current : false,
                },
                {
                    text : "Videos",
                    url : "#",
                    current : false,
                },
                {
                    text : "News",
                    url : "#",
                    current : false,
                }],

            listShop : [
                {
                    text : "Shop DC",
                    url : "#",
                    current : false,
                },
                {
                    text : "Shop DC Collectibles",
                    url : "#",
                    current : false,
                }],

            listDC : [
                {
                    text : "Terms of use",
                    url : "#",
                    current : false,
                },
                {
                    text : "Privacy policy (New)",
                    url : "#",
                    current : false,
                },
                {
                    text : "Ad Choices",
                    url : "#",
                    current : false,
                },
                {
                    text : "Advertising",
                    url : "#",
                    current : false,
                },
                {
                    text : "Jobs",
                    url : "#",
                    current : false,
                },
                {
                    text : "Subscriptions",
                    url : "#",
                    current : false,
                },
                {
                    text : "Talent Workshops",
                    url : "#",
                    current : false,
                },
                {
                    text : "CPSP Certificates",
                    url : "#",
                    current : false,
                },
                {
                    text : "Ratings",
                    url : "#",
                    current : false,
                },
                {
                    text : "Shop Help",
                    url : "#",
                    current : false,
                },
                {
                    text : "Contact Us",
                    url : "#",
                    current : false,
                }],

            listSites : [
                {
                    text : "DC",
                    url : "#",
                    current : false,
                },
                {
                    text : "MAD Magazine",
                    url : "#",
                    current : false,
                },
                {
                    text : "DC Kids",
                    url : "#",
                    current : false,
                },
                {
                    text : "DC Universe",
                    url : "#",
                    current : false,
                },
                {
                    text : "DC Power Visa",
                    url : "#",
                    current : false,
                }
                ],



        }
    }
}
</script>

<style scoped>
    ul {
        list-style: none;
        text-decoration-style: none;
       
    }

    a {
        text-decoration: none;
        color: gray;
    }
</style>