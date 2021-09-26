<template>
  <header>
      <div class="">
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

<style>
    ul {
        list-style: none;
        text-decoration-style: none;
        float: right;
        display: flex;
        justify-content: flex-end;
    }

    .header_logo {
        float: left;
        margin: -30px 0 -30px 100px;
    }

    li {
       padding-right: 15px;
       
    }

    a {
        text-decoration: none;
        text-transform: uppercase;
        color: black;
        font-weight: bold;
    }

    .header_section {
        padding: 30px;
    }
</style>