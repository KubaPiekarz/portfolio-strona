<template>
    <section id="projects">
        <h1>My projects</h1>
        <div class="project">
            <div class="text">
                <h3>Pokemon App</h3>
                <p>I created it using technologies such as Vue.js, Vuex, Axios, and Tailwind CSS. The application allows
                    browsing information about various Pokemon, managing a favorites list, and also includes dynamic
                    display of data from external APIs. The project is continuously being expanded, and the current
                    source code can be found on my GitHub.</p>
            </div>
            <a href="https://pokemon-seven-umber.vercel.app/" target="_blank">

                <img :src="Laptop" alt="Pokemon App">
                <img :src="Mobile" alt="Pokemon App">

            </a>
        </div>
    </section>
</template>
<script setup>
import Laptop from '../assets/laptop.png'
import Mobile from '../assets/mobile.png'




</script>


<style scoped>
section {
    padding: 2em;
    background-color: #fffffa;
    @media screen and (max-width: 767px) {
        padding: 0;
    }

}

a {
    text-decoration: none;
    color: black;
    z-index: 2;
}

h1 {
    font-size: 4em;
    margin-bottom: 20px;
    color: #0d5c63;
    text-align: center;
    border-bottom: 2px solid #78cdd7;
    @media screen and (max-width: 767px) {
        font-size: 50px;
    }

}

.text {
    width: 70%;
    margin: auto;
    margin-bottom: 50px;
}

.project {
    text-align: center;
}

img {
    width: 100%;
    max-width: 600px;
    z-index: -1;
}
</style>