<template>
    <div class="navigation">
        <div class="btn">About me</div>
        <div class="btn">Contacts</div>
    </div>
</template>

<script>

    export default {
        name:"navigationComponent"
    

}
</script>

<style>
    .navigation
    {
        display:flex;
        flex-direction: row;
        width:30%;
        justify-content: space-around;
        font-family: "Play", sans-serif;
        font-weight: 600;
        top:10vh;
        position: relative;
        height: 10%;
    }

    .btn:hover{
        cursor: pointer;
    }

</style>