<template>
  <header>
      <div class="header_wrap">
        <a href="#" class="header_logo">
            <img src="../assets/vue-dc-comics-1/img/dc-logo.png" alt="dc logo">
        </a>

        <nav>
            <ul>
                <li v-for="(element, index) in listElements" :key="index">
                    <a :class={active:listElements.current} href="">{{element.text}}</a>
                </li>
            </ul>
        </nav>
      </div>
  </header>
</template>

<script>
export default {
    name : 'Header',
    data : function () {
        return { //ciò che normalmente scriveremmo nel data
            index : 0,
            listElements : [
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
                    text : "Collectibles",
                    url : "#",
                    current : false,
                },
                {
                    text : "videos",
                    url : "#",
                    current : false,
                },
                {
                    text : "Fans",
                    url : "#",
                    current : false,
                },
                {
                    text : "News",
                    url : "#",
                    current : false,
                },
                {
                    text : "Shop",
                    url : "#",
                    current : false,
                },


                
                
                
                
                
                ]

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
       
    }

    .header_logo {
        margin: -30px 0 -30px 0;
    }

    li {
        padding-right: 15px;
        display: inline-block;
         
    }

    a {
        text-decoration: none;
        text-transform: uppercase;
        color: $blackColor;
        font-weight: bold;

        &:active {
        color: $dcLogoColor;
            .div-line-nav {
            background-color: $dcLogoColor;
            height: 2px;
            width: 30px;
            }
        }
    }

    .header_wrap {
        display: flex;
        justify-content: space-between;
        padding: 50px 100px 40px 100px;
    }

</style>