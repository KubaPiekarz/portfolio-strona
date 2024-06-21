<template>
    <section id="tech-stack">
      <h1>My technology stack</h1>
      <div class="tech-list">
        <span v-for="tech in techStack" :key="tech">{{ tech }}</span>
      </div>
    </section>
  </template>
  
  <script setup>
  const techStack = [
    'HTML', 'CSS', 'JavaScript', 'Typescript', 'Vue.js', 'Vuex', 'Pinia', 
    'Axios', 'Quasar', 'Sass', 'Tailwind', 'Bootstrap', 'Git', 'Figma', 
    'Adobe XD', 'Illustrator', 'Photoshop'
  ];
  </script>
  
  <style scoped>
  section {
    text-align: center;
    padding: 4em 0;
    color: #fffffa;
    background-color: #fffffa;

  }

  h1{
    font-size: 4em;
    border-bottom: 2px solid #78cdd7;
    margin-bottom: 20px;
    color: #0d5c63;
    @media screen and (max-width: 767px) {
        font-size: 50px;
    }
  }
  .tech-list {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
  .tech-list span {
    background-color: #4dd0e1;
    margin: 0.5em;
    padding: 1em 3em;
    border-radius: 4px;
  }
  </style>