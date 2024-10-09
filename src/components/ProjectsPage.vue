<template>
  <div class="projects-container">
    <!-- Projects Grid -->
    <div class="projects-grid">
      <div class="project-card" v-for="(project, index) in projects" :key="index" @click="goToProject(project.link)">
          <h2>{{ project.title }} →</h2>
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
        { title: 'Project 1', description: 'Project Description', link: 'https://example1.com' },
        { title: 'Project 2', description: 'Project Description', link: 'https://example2.com' },
        { title: 'Project 3', description: 'Project Description', link: 'https://example3.com' },
        { title: 'Project 4', description: 'Project Description', link: 'https://example4.com' },
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
  transition: background 1.5s, color 1.5s;
}

.project-card:hover {
  /* Highlight effect on hover */
  color: black; 
  background: white

}

.project-card h2 {
  font-size: 20px;
  margin-bottom: 10px;
}

.project-card p {
  font-size: 16px;
  margin: 0;
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
  font-size: 16px;
  transition: background-color 0.3s;
}

.back-link:hover {
  background-color: white;
  color: black;
}
</style>
