<template>
    <section id="who-am-i">
        <img :src="Shape" />
        <div class="content">
            <h1>Who am I?</h1>
            <p>I am a seasoned front-end developer proficient in Vue.js, boasting over two years of hands-on experience in
                crafting dynamic and responsive web applications. My journey in web development has equipped me with a deep
                understanding of Vue.js framework, allowing me to efficiently build elegant and efficient user interfaces.
    
                In addition to my technical expertise, I am also dedicated to continuous learning and improvement.
                Currently, I am expanding my skill set by pursuing studies in graphic design. This dual focus allows me to
                marry my passion for both technology and creativity, enabling me to bring innovative and visually appealing
                solutions to life.</p>
        </div>
    </section>
</template>
<script setup>
import Shape from '../assets/shape1white.svg'

</script>
<style scoped>
section {
    background-color: #44A1A0;
    height: 50vh;
    padding: 2em 10em 2em 0;
    position: relative;
    color: #fffffa;
    @media screen and (max-width: 767px) {
        padding: 10px 20px 0 0; 
        height: 100%;
    }
}

img{
    position: absolute;
    left: 0;
    bottom: 0;
    @media screen and (max-width: 767px) {
        transform: scale(0.25, 0.25);
        transform-origin: left;
    }
}

svg{
    fill: white !important;
    color: aliceblue;
    background-color: aliceblue;
}

.content{
    width: 40%;
    margin-left: auto;
    @media screen and (max-width: 767px) {
        width: 60%;

    }
}

h1{
    font-size: 4em;
    border-bottom: 2px solid #78cdd7;
    margin-bottom: 10px;
    color: #0d5c63;
    @media screen and (max-width: 767px) {
        font-size: 30px;
    }
}
</style>