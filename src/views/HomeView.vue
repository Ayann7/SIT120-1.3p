<template>
  <section class="home-page">
    <div class="intro">
      <h1>Hello and Welcome to my Portfolio!</h1>
      <p>My name is Ayan, I am 19 years old and currently studying Bachelor of Information Technology</p>
      <p>Explore my work, learn about my skills, and feel free to reach out for collaborations or inquiries.</p>
      <button @click="showProjects">View my Projects</button>
    </div>
    <div class="project-list" v-if="projectsVisible">
    <h2>My Projects</h2>
    <ul>
      <li>
        <h3>
          <a href="https://github.com/Ayann7/SIT120-1.1p" target="_blank">Project 1 <br>
          <img src="1.1p-ss.png" alt="Project 1" height="120" width="260">
        </a>
        </h3>
        <p>This project was about basic html and css. I have used basic html elements in this project such as lists, images, tables and more!</p>
      </li>
      <li>
        <h3>
          <a href="https://github.com/Ayann7/FootballProj" target="_blank">Project 2 <br>
          <img src="football-ss.png" alt="Project 2" height="120" width="260">
        </a>
        </h3>
        <p>This project was about the basics of Football. It uses basic HTML, CSS and JavaScript. In the end a feedback form is present too, feel free to send me your feedback! Please click the image above to access the project</p>
      </li>
      <li>
        <h3>
          <a href="https://github.com/Ayann7/SIT120---2.2c" target="_blank">Project 3 <br>
          <img src="proj3-ss.png" alt="Project 3" height="125" width="260">
        </a>
        </h3>
        <p>This project was about a car renting model website. I have used HTML, CSS and VUE3 concepts for this website. Please click the image above to access the project</p>
      </li>
    </ul>
  </div>
  </section>
</template>

<script setup>
import { ref } from 'vue';

const projectsVisible = ref(false);

const showProjects = () => {
  projectsVisible.value = true;
};
</script>

<style scoped>
</style>
