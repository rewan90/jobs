<template>
<div id="nav">
    <router-link to="/">Home</router-link>
    <router-link :to="{ name: 'About' }">About</router-link>
    <router-link :to="{ name: 'Jobs' }">Jobs</router-link>
    <router-link :to="{ name: 'signUp' }">Sign Up</router-link>
</div>

<router-view />
</template>

<script>
import signUp from './components/signUp.vue'
export default {
  name: 'App',
  components: { }
}
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    max-width: 960px;
    margin: 0 auto;
}

#nav {
    padding: 30px;
}

#nav a {
    font-weight: bold;
    color: #2c3e50;
    text-decoration: none;
    padding: 10px;
    border-radius: 4px;
}

#nav a.router-link-exact-active {
    color: white;
    background: crimson;
}
</style>
