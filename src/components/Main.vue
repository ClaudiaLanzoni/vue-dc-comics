<template>
    <main class="main_section">
        <h2> &lt; -- Content goes here -- &gt; </h2>
    </main>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>

@import "../style/variables.scss";
@import "../style/general.scss";

    h2 {
        color: $whiteColor;
    }

    .main_section {
        background-color: $blackColor;
        height: 100px;
        display: flex;
        align-items: center;
        padding: 60px 100px 60px 100px;
    }
</style>