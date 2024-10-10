<template>
  <div class="projects-container">
    <!-- Projects Grid -->
    <div class="projects-grid">
      <div class="project-card" v-for="(project, index) in projects" :key="index" @click="goToProject(project.link)">
        <h1>{{ project.title }} →</h1>
        <p>{{ project.description }}</p>
      </div>
    </div>

    <div class="back-button">
      <router-link to="/" class="back-link">← Back</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Projects',
  data() {
    return {
      projects: [
        { title: 'Glowing Bud Admin Platform', description: 'An admin platform which allows the clients to see details on their users, add/update data plans, manage e-sim inventory and track telemetry data.', link: 'https://app.glowingbud.com' },
        { title: 'Glowing Bud E-sim Application', description: 'A web/mobile app which enables users to purchase travel e-sims and manage data plans, it supports multiple countries and regions based on individual clients requirments.', link: 'https://www.glowingbud.com/white-label-esim-web-application/' },
        { title: 'String', description: 'A basic chat application built by me in 2021. I recently updated it using vuejs and deployed on netlify.', link: 'https://cool-banoffee-1bc218.netlify.app/' },
      ],
    };
  },
  methods: {
    goToProject(link) {
      window.open(link, '_blank');
    },
  },
};
</script>

<style scoped>
/* General page styling */
.projects-container {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 100vh;
  color: white;
  background-color: #111;
  padding: 20px;
}

header {
  background-color: #ffffff;
  padding: 10px;
}

/* Flexbox for the navigation bar */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.social-icons {
  display: flex;
}

.social-icons img {
  width: 24px;
  height: 24px;
  margin-left: 10px;
}

nav span {
  font-size: 24px;
  font-weight: bold;
}

/* Projects grid styling */
.projects-grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  /* Creates two columns */
  gap: 20px;
  /* Space between cards */
  flex-grow: 1;
}

.project-card {
  border: 2px solid white;
  padding: 20px;
  text-align: left;
  cursor: pointer;
  /* Make cards look clickable */
  transition: background 0.7s, color 0.7s;
}

.project-card:hover {
  /* Highlight effect on hover */
  color: black;
  background: white
}

.project-card h1 {
  font-size: 30px;
  margin: 10px;
}

.project-card p {
  font-size: 20px;
  margin: 10px;
}

/* Back button styling */
.back-button {
  text-align: center;
  margin-top: 20px;
}

.back-link {
  display: inline-block;
  padding: 10px 20px;
  border-radius: 25px;
  border: 1px solid white;
  color: white;
  text-decoration: none;
  font-size: 18px;
  transition: background-color 0.3s;
}

.back-link:hover {
  background-color: white;
  color: black;
}
</style>
