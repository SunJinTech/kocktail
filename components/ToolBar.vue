<template>
  <div class="toolbar-container">
    <div class="logo-container">
      <img class="logo" src="https://img.icons8.com/nolan/96/cocktail.png" />
      <span class="title">콕!테일</span>
    </div>
    <div class="nav">
      <nuxt-link to="/home">Home</nuxt-link>
      <nuxt-link to="/recipe">Recipe</nuxt-link>
      <nuxt-link to="/mypage">Mypage</nuxt-link>
    </div>
    <div class="auth-nav">
      <nuxt-link to="/login">Sign In</nuxt-link>
      <nuxt-link to="/signup">Sign Up</nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
}
</script>

<style scoped>
.toolbar-container {
  padding: 20px;
  /* background-color: rgba(252, 84, 109, 0.37); */
  background-color: rgba(58, 52, 53, 0.9);
  display: flex;
}

.logo-container {
  flex-grow: 1;
  margin: 0 10px;
  align-items: center;
}
.logo {
  height: 31px;
}
.title {
  font-weight: bold;
  font-size: 1.5em;
  color: white;
  text-shadow: 1px 1px 2px rgb(58, 52, 53), 0 0 15px white,
    0 0 5px rgb(252, 84, 109);
}
.nav {
  display: flex;
  margin: 10px 0;
  justify-content: space-evenly;
  flex-grow: 4;
}

.nav a {
  font-weight: bold;
  color: white;
  text-decoration: none;
}

.nav a.router-link-exact-active {
  color: rgb(252, 84, 109);
}

.auth-nav {
  flex-grow: 1;
  margin: 10px;
}

.auth-nav a {
  color: white;
  margin: 0 10px;
  text-decoration: none;
  padding: 5px;
}
.auth-nav a.router-link-exact-active {
  border: 1px solid white;
  border-radius: 5px;
}
</style>