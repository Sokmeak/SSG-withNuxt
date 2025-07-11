<template>
  <div class="about-container">
    <div class="content-box">
      <h1>About Us</h1>
      <p>
        Welcome to our website! We are passionate about building great user
        experiences and sharing knowledge with the world.
      </p>
      <p>
        Our mission is to create meaningful solutions, inspire innovation, and
        connect people through technology.
      </p>
    </div>

    <NuxtLink to="/" class="link-button">Back to Home Page</NuxtLink>
  </div>
</template>

<script>
import { NuxtLink } from "#components";

export default {
  name: "AboutPage",
};
</script>

<style scoped>
.about-container {
  display: flex;
  flex-direction: column;
  gap: 1rem;
  align-items: center;
  justify-content: center;
  padding: 80px 20px;
  background: linear-gradient(to right, #e3f2fd, #fce4ec);
  min-height: 100vh;
}

.content-box {
  max-width: 700px;
  background-color: white;
  padding: 40px;
  border-radius: 15px;
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
  animation: fadeIn 1s ease;
  text-align: center;
}
.link-button {
  padding: 12px 24px;
  background-color: #42b983;
  color: white;
  text-decoration: none;
  border-radius: 6px;
  font-weight: bold;
  transition: background-color 0.3s ease, transform 0.2s ease;
}

h1 {
  font-size: 3em;
  color: #3f51b5;
  margin-bottom: 20px;
}

p {
  font-size: 1.2em;
  color: #555;
  line-height: 1.6;
  margin-bottom: 15px;
}

@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(40px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>
