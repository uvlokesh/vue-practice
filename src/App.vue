<template>
  <div id="nav">
    <router-link to="/">Home</router-link>
    <router-link to="/about">About</router-link>
  </div>
  <div class="container">
    <router-view />
  </div>
</template>


<style>
#nav {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 1rem 0;
}

#nav a {
  margin: 0 10px;
  text-decoration: none;
  font-size: 24px;
  color: rgb(24, 25, 8);
}

#nav a.router-link-active {
  color: green;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}
</style>
