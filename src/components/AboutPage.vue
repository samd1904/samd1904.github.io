
<!-- src/views/AboutMe.vue -->
<template>
  <div class="about-container">
    
    <div class="content">
      <div class="about-me">
        <p>
          I’m a passionate Node.js backend developer with a strong focus on building scalable, high performance applications. I thrive on solving complex problem statements and designing efficient solutions. I aim to create clean, maintainable code that powers seamless user experiences.
        </p>
        <p>
          My enthusiasm for backend technologies goes beyond coding, I enjoy learning about new frameworks, database management, and architectural patterns that can elevate my solutions to the next level. Always curious and adaptable, I’m constantly pushing my limits to become a better developer and solve the toughest problems.
        </p>
      </div>
      <div class="work-experience">
        <h2>Work Experience</h2>
        <ul>
          <li>
            <b>Position</b><br />
            Company Name<br />
            Job Description
          </li>
          <li>
            <b>Position</b><br />
            Company Name<br />
            Job Description
          </li>
        </ul>
      </div>
    </div>

    <div class="back-button">
      <router-link to="/" class="back-link">← Back</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AboutMe',
};
</script>

<style scoped>
/* General page styling */
.about-container {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 100vh;
  color: white;
  background-color: #111;
  padding: 20px;
}

header {
  display: flex;
  justify-content: space-between;
  padding: 10px;
  background-color: #ffffff;
  color: #000000;
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

/* Content styling */
.content {
  display: flex;
  justify-content: space-between;
  flex-grow: 1;
}

.about-me {
  width: 60%;
  font-size: 16px;
}

.work-experience {
  width: 30%;
}

.work-experience h2 {
  font-size: 20px;
  margin-bottom: 10px;
}

.work-experience ul {
  list-style-type: none;
  padding: 0;
}

.work-experience li {
  margin-bottom: 20px;
  line-height: 1.6;
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
