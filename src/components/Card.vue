<template>
  <div class="card_element">
            <div></div>
        </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

@import "../style/variables.scss";
@import "../style/general.scss";

    .card_element {
        height: 100px;
        width: 100px;
        background-color: rgb(46, 224, 224);
        border: 5px solid black;
        flex-basis: calc(100% / 6);
        margin: 0 auto
    }
</style>