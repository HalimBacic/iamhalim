<template>
    <div class="imagebox">

    </div>
</template>

<script>
    export default {
        name:"GraphComponent",
    }
</script>

<style scoped>
.imagebox
{
    background-image: url('../assets/duotone.jpg');
    height: 55vh;
    width: 60vw;
    background-position: center;
    background-size:cover;
    position: relative;
    top:10vh;
    left:8vw;
    z-index: -10;
}
</style>