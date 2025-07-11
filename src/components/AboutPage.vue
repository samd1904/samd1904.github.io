<!-- src/components/AboutPage.vue -->
<template>
  <div class="about-container">
    <div class="content">
      <div class="about-me">
        <p>
          I’m a passionate Node.js backend developer with a strong focus on building scalable, high-performance
          applications. I thrive on solving complex problem statements and designing efficient solutions. I aim to
          create clean, maintainable code that powers seamless user experiences.
        </p>
        <p>
          My enthusiasm for backend technologies goes beyond coding, I enjoy learning about new frameworks, database
          management, and architectural patterns that can elevate my solutions to the next level. Always curious and
          adaptable, I’m constantly pushing my limits to become a better developer and solve the toughest problems.
        </p>
        <p>
          Collaboration is also at the core of my work. I believe in the power of teamwork and open communication to
          achieve shared goals. I love participating in code reviews and brainstorming sessions with my peers, where I
          can both share my knowledge and learn from others. This exchange of ideas and perspectives allows me to refine
          my skills and stay at the forefront of backend development trends.
        </p>
        <p>
          Moreover, I have a strong interest in DevOps practices and automation. I’m passionate about streamlining
          development workflows, improving deployment pipelines, and ensuring high availability and performance of the
          systems I build. With an ever-growing interest in cloud infrastructure, I’m working towards deepening my
          expertise in cloud-native technologies like Kubernetes and serverless architectures.
        </p>
      </div>
      <div class="work-experience">
        <h1>Work Experience</h1>
        <ul style="list-style: none; padding-left: 0; line-height: 2em;">
          <li style="margin-bottom: 2em;">
            <h3 style="margin: 0; font-size: 1.3em; font-weight: bold;">&#x2022; SAP UI 5 Consultant</h3>
            <p style="margin: 0; font-size: 1em; font-weight: 400;">
              <b>- Crave Infotech Pvt. Ltd. (2020-2022)</b><br />
              <span style="font-size: 0.9em;">
                Responsible for developing web and mobile applications using the SAP UI5 hybrid app framework and
                working with Appcelerator native app framework.
              </span>
            </p>
          </li>
          <li style="margin-bottom: 2em;">
            <h3 style="margin: 0; font-size: 1.3em; font-weight: bold;">&#x2022; Node JS Developer</h3>
            <p style="margin: 0; font-size: 1em; font-weight: 400;">
              <b>- Solulab Pvt. Ltd. (2022-2023)</b><br />
              <span style="font-size: 0.9em;">
                Developed Backend APIs using blockchain technologies and Node.js for NFT-based projects.
              </span>
            </p>
          </li>
          <li>
            <h3 style="margin: 0; font-size: 1.3em; font-weight: bold;">&#x2022; Senior Software Developer Level-3 (SDE 3)</h3>
            <p style="margin: 0; font-size: 1em; font-weight: 400;">
              <b>- Glowing Bud Pvt. Ltd. (2023-2024)</b><br />
              <span style="font-size: 0.9em;">
                Built scalable and reliable Backend for a travel eSIM retail application and a CRM platform to manage
                users, data plans, and inventory for administrators.
              </span>
            </p>
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
  height: 100%;
  color: white;
  background-color: #111;
  padding: 20px;
  overflow-y: auto;
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

p {
  font-size: 24px;
}

br {
  margin: 0.5em 0;
  /* FF for instance */
  line-height: 2em;
  /* chrome for instance */
}

li {
  font-size: 24px;
}

/* Content styling */
.content {
  display: flex;
  justify-content: space-between;
  flex-grow: 1;
  overflow-y: auto;
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
  font-size: 18px;
  transition: background-color 0.3s;
}

.back-link:hover {
  background-color: white;
  color: black;
}

/* Media Queries */
@media (max-width: 768px) {
  .content {
    flex-direction: column;
  }

  .about-me, .work-experience {
    width: 100%;
  }

  p, li {
    font-size: 18px;
  }

  .back-link {
    font-size: 16px;
  }
}
</style>
