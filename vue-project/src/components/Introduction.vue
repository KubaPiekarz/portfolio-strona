<template>
    <section id="introduction">
        <header>
            <nav>
                <ul>
                    <li><a href="#experience">Experience</a></li>
                    <li><a href="#tech-stack">Tech stack</a></li>
                    <li><a href="#projects">Projects</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
            <img class="shape" :src="Shape" />
        </header>
        <div class="content" >
            <div class="header">
                <h1>Hello, <br /> I'm Jakub!</h1>
    
                <img class="icon" :src="Icon"></img>
            </div>
            <p>I am a driven front-end developer who thrives on tackling new challenges head-on. With a keen eye for design,
                I am passionate about crafting intuitive and visually striking modern web applications. I find joy in
                bringing ideas to life through clean, efficient code and seamless user experiences.</p>
        </div>


    </section>
</template>
<script setup>
import Icon from '../assets/icon1.svg'
import Shape from '../assets/shape1.svg'

</script>

<style scoped>
section {
    /* width: 50%; */
    height: 100vh;
    position: relative;
    background-color: #FFFFFA;
}
header {
    padding: 1em;
    width: 40%;
    margin-left: auto;
    @media screen and (max-width: 767px) {
        width: 100%;
        padding: 0;
    }
}

.icon{
    height: 150px;
}

nav{
    position: relative;
    z-index: 2;
    @media screen and (max-width: 767px) {
        padding-top: 20px;
        
    }
}
.shape{
    position: absolute;
    top: -50px;
    right: 0;
    z-index: 0;
    @media screen and (max-width: 767px) {
        top: -150px;
    }
}

nav ul {
    list-style: none;
    display: flex;
    justify-content: space-around;
}

a {
    z-index: 2;
    text-decoration: none;
    color: #00695c;
    font-weight: bold;
    cursor: pointer;
}

.content{
    width: 50%;
    padding-left: 200px;
    position: absolute;
    top: 300px;

    @media screen and (max-width: 767px) {
        width: 100%;
        padding: 0 50px;
    }
}

.header {
    display: flex;
    align-items: center;
    gap: 20px;
    margin-bottom: 20px;
}


h1 {
    font-size: 4em;
    @media screen and (max-width: 767px) {
        font-size: 50px;
    }
}
</style>