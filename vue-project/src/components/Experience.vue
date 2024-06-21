<template>
    <section id="experience">
        <div>
            <img class="shape" :src="Shape" />
            <div class="content">
                <h1>My experience</h1>
                <ul>
                    <li>
                        <h3>Junior Frontend Developer - Futurum Technology Ltd (Kraków)</h3>
                        <p>1.09.2022 - Present</p>
                        <ul>
                            <li>Active participation in projects using Vue.js, Vuex, Axios,
                                and Sass to create functional and aesthetically pleasing
                                user interfaces.
                                Collaboration with the project team and involvement in
                                the design, implementation, and optimization of web
                                applications.
                                Implementation and customization of Vue components
                                and state management using Vuex.
                                Optimizing website performance, ensuring minimal
                                loading times and optimized code.
                                Creating and maintaining style sheets in Sass to ensure
                                visual consistency in projects. Integration with external
                                APIs using Axios to enable dynamic data display on
                                pages.
                                Resolving ongoing issues and participating in
                                application testing to improve product quality and
                                reliability.</li>
                        </ul>
                    </li>
                    <div class="rightSide">
                        <li>
                            <h3>Web Developer - MasterApps</h3>
                            <p>1.07.2022 - 31.08.2022</p>
                        </li>
                        <li>
                            <h3>Trainee - Itransition Group</h3>
                            <p>1.04.2022 - 31.05.2022</p>
                        </li>
                    </div>
                </ul>
            </div>
        </div>
        <img class="shape1" :src="Shape2" />

    </section>
</template>
<script setup>
import Shape from '../assets/shape2.svg'
import Shape2 from '../assets/shape1white.svg'



</script>

<style scoped>
section {
    background-color: #44A1A0;
    height: 90vh;
    position: relative;
    padding: 2em 0 2em 30em;
    color: #fffffa;

    @media screen and (max-width: 767px) {
        padding: 10px 0 0 20px; 
        height: 100%;
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

h3{
    font-size: 1.4em;
    color: #0d5c63;
    @media screen and (max-width: 767px) {
        font-size: 20px;
    }
}

.content {
    width: 40%;
    @media screen and (max-width: 767px) {
        width: 60%;
    }
}

.rightSide{
    position: absolute;
    margin-top: 50px;
    left: 30%;
    @media screen and (max-width: 767px) {
        position: unset;
        padding-bottom: 20px;
    }
}

.shape {
    position: absolute;
    right: 0;
    @media screen and (max-width: 767px) {
        transform: scale(0.25, 0.25);
        transform-origin: right;
    }
}

.shape1 {
    position: absolute;
    left: 0;
    bottom: 20px;
    height: 500px;
    @media screen and (max-width: 767px) {
        display: none;
    }
}

ul {
    list-style: none;
    padding: 0;
}
</style>