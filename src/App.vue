<template>
  <div id="app">
    <Profile />
  </div>
</template>

<script>
import Profile from './components/Profile';

export default {
  name: 'app',
  components: {
    Profile
  }
}
</script>

<style>
body {
  background-color: #001947;
  color: #ffffff;
  text-align: center;
  padding: 0rem;
  margin: 0rem;
  font-family: 'Courier New', Courier, monospace;
}

.profile-pic img {
  width: 250px;
  border-radius: 10%;
}

.stuff ul {
  list-style: none;
  padding-left: 0;
  font-size: 1.5rem;
  margin: 0 auto;
  width: 30%;
  background-color: #ffffff;
  color: #001947;
}

.stuff ul li {
  border: 1px solid #001947;
  padding: 1rem;
  text-transform: capitalize;
}

footer {
  position: fixed;
  width: 100%;
  bottom: 0rem;
  padding: 1rem;
  border-top: 1px solid #ffffff;
}
</style>
