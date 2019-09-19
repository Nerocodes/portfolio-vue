<template>
  <div id="app">
    <Profile />
    <div class="sections">
      <Frontend />
      <Backend />
      <Works />
      <Social />
    </div>
  </div>
</template>

<script>
import Profile from './components/Profile';
import Frontend from './components/Frontend';
import Backend from './components/Backend';
import Social from './components/Social';
import Works from './components/Works';

export default {
  name: 'app',
  components: {
    Profile,
    Frontend,
    Backend,
    Works,
    Social
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

.sections section {
  margin: 0 auto;
  width: 30%;
  background-color: #ffffff;
  color: #001947;
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
