<template>
    <section id="contact">
      <h1>Contact</h1>
      <p>If you have any questions, business inquiries, or just want to chat, feel free to reach out!</p>
      <div class="social-links">
        <a href="https://www.linkedin.com/in/jakub-piekarz-96a2b9235/">
            <img :src="LinkedIn"
        </a>
        <a href="https://www.instagram.com/piekixo/?hl=pl">
            <img :src="Instagram"
        </a>
        <a href="https://github.com/KubaPiekarz">
            <img :src="Github"
        </a>
      </div>
      <img class="shape" :src="Shape2"/>
      <img class="shape2" :src="Shape2"/>

    </section>
  </template>
<script setup>
import Shape from '../assets/shape2.svg'
import Shape2 from '../assets/shape1white.svg'
import Instagram from '../assets/instagram.svg'
import LinkedIn from '../assets/linkedin.svg'
import Github from '../assets/github.svg'

</script>
  
  <style scoped>
  section {
    background-color: #44A1A0;
    text-align: center;
    padding: 2em;
    color: #FFFFFA;
    position: relative;
    height: 70vh;
    overflow: auto;
    @media screen and (max-width: 767px) {
           height: 100%;
        }
    p{
        font-size: 30px;
        width: 40%;
        margin: 50px auto;
        @media screen and (max-width: 767px) {
            font-size: 20px;
            width: 100%;
        }

    }
  }
  h1{
    font-size: 4em;
    margin-bottom: 10px;
    @media screen and (max-width: 767px) {
        font-size: 50px;
    }

  }
  .social-links {
    display: flex;
    justify-content: center;
    gap: 1em;
    img{
        height: 50px;
    }
  }

  .shape{
    position: absolute;
    left: 0;
    bottom: 0;
    @media screen and (max-width: 767px) {
        display: none;
    }
  }

  .shape2{
    position: absolute;
    right: 0;
    bottom: 0;
    transform: rotate(180deg);
    z-index: 0;
    @media screen and (max-width: 767px) {
        display: none;

    }

  }

  </style>