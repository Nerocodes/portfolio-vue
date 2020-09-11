<template>
  <div id="app">
    <Profile />
    <div class="sections">
      <Frontend />
      <Backend />
      <Works />
      <Social />
    </div>
    <Footer />
  </div>
</template>

<script>
import Profile from './components/Profile';
import Frontend from './components/Frontend';
import Backend from './components/Backend';
import Social from './components/Social';
import Works from './components/Works';
import Footer from './components/Footer';

export default {
  name: 'app',
  components: {
    Profile,
    Frontend,
    Backend,
    Works,
    Social,
    Footer
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
  overflow-x: hidden;
}

.profile-pic img {
  width: 300px;
  height: 300px;
  border-radius: 50%;
  object-fit: contain;
}

.sections section {
  margin: 0 auto;
  width: 30%;
  min-width: 250px;
  background-color: #ffffff;
  color: #001947;
  border: 1px solid #001947;
  padding: 1rem;
  text-transform: capitalize;
}

footer {
  position: relative;
  width: 100%;
  bottom: 0rem;
  padding: 1rem 0rem;
}
</style>
