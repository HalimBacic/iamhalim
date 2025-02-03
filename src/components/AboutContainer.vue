<template>
    <div class="container">
            <div class="left">
                <img class="imageclass" src="../assets/cv slika.jpg">
            </div>
            <div class="right">
                I am Halim, 29 years old. I am a software developer with a background in backend development using .NET. 
                I was born in Gradiška, Bosnia and Herzegovina, in 1995 and currently reside and work in Banja Luka. 
                My expertise includes Java, Spring, C, C++, React, and Android development, with ongoing self-learning in Python. 
                I have experience working with MySQL databases.
            </div>
    </div>
</template>

<script>

    export default {
        name:"AboutContainer"

}
</script>

<style scoped>
    div
    {
        width:100vw;
        height:70%;
    }

    .container
    {
        display: flex;
        flex-direction: row;
    }

    .left
    {
        width: 35%;
    }

    .right
    {
        width:65%;
        font-family: 'Nunito', sans-serif;
        font-size: 25px;
        font-weight: 400;
        display: grid; 
        place-items: center; 
        padding: 10%;
    }

    .imageclass
    {
        border-radius: 15%;
        height:40vh;
        width:20vw;
        margin-top:18vh;
    }

</style>