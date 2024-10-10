<template>
  <div class="home">
    <div class="intro">
      <p>Hi.</p>
      <p>I am Saumya Darne</p>
      <p>I am a Backend Developer</p>
      <p>Welcome to my portfolio</p>
    </div>
    <div class="buttons">
      <router-link to="/projects">
        <button>Projects →</button>
      </router-link>
      <router-link to="/about">
        <button>About Me →</button>
      </router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomePage',
};
</script>

<style scoped>
.home {
  display: flex;
  flex-direction: column;
  background-color: #111;
  justify-content: center;
  align-items: center;
  height: 100%;
}

.intro {
  text-align: center;
  font-size: 24px;
  color: white;
}

.buttons {
  display: flex;
  justify-content: center;
  margin-top: 20px;
}

button {
  margin: 10px;
  padding: 10px 20px;
  border: 2px solid black;
  border-radius: 50px;
  font-size: 18px;
  background-color: white;
  cursor: pointer;
  width: 150px;
  transition: background 0.3s, color 0.3s, border 0.3s
}

button:hover{
  color: white;
  background-color: #111;
  border: 2px solid white;
}
</style>
