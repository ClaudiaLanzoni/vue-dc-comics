<template>
    <div>
        <div class="card_element">
            <div>
                <img class="card_img_container" :src="thumb">
            </div>
        </div>

        <div class="series_name_container">
            <div class="series_name_style">{{series}}</div>
        </div>
        
    </div>
</template>

<script>
export default {
    name: 'Card',
    //props: ['thumb', 'series']

    props : { //meglio perchè "documenta" il tipo di informazione
        thumb : String,
        series : String
    }
}
</script>

<style lang="scss" scoped>

@import "../style/variables.scss";
@import "../style/general.scss";

    .card_element {
        //flex-basis: calc(100% / 6);
        margin: 20px;
        height: 150px;
        width: 150px;
        overflow: hidden;
        //word-wrap: break-word; 
    }

    .card_img_container {
        height: 100%;
        width: 100%;
    }

    .series_name_style {
        //font-family: $seriesFont;
        font-size: 12px;
        text-transform: uppercase;
        text-align: center;
        color: $whiteColor;
        
    }
</style>