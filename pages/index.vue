<template>
  <div class="homepage">
    <h1>Welcome to My Website</h1>
    <p>Click below to learn more about us.</p>
    <NuxtLink to="/about" class="link-button">Visit About Page</NuxtLink>
  </div>
</template>

<script>
export default {
  name: "HomePage",
};
</script>

<style scoped>
.homepage {
  text-align: center;
  padding-top: 10%;
  background: linear-gradient(to right, #e0f7fa, #f1f8e9);
  height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

h1 {
  font-size: 3em;
  color: #333;
  margin-bottom: 10px;
}

p {
  font-size: 1.2em;
  color: #555;
  margin-bottom: 30px;
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

.link-button:hover {
  background-color: #2c9e74;
  transform: scale(1.05);
}
</style>
