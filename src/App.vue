<!-- src/App.vue -->
<template>
  <div id="app">
    <header>
      <nav>
        <span>Hello World!</span>
        <div class="social-icons">
          <a href="https://www.linkedin.com" target="_blank">
            <img src="@/assets/linkedin-icon.png" alt="LinkedIn" />
          </a>
          <a href="https://www.github.com" target="_blank">
            <img src="@/assets/github-icon.svg" alt="GitHub" />
          </a>
        </div>
      </nav>
    </header>
    <router-view />
  </div>
</template>

<script>
export default {
  name: 'App',
};
</script>

<style>
/* Basic styling for header and social icons */

html, body {
  margin: 0;
  padding: 0;
  height: 100%;
  width: 100%;
  box-sizing: border-box;
}

#app {
  font-family: 'JetBrains Mono', monospace;
  color: white;
  height: 100vh;
  margin: 0;
  display: flex;
  flex-direction: column;
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
</style>
