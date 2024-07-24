<template>
  <section class="socials">
    <div class="linkedIn">
      <a href="https://www.linkedin.com/in/nerocodes" target="blank"><i class="fab fa-linkedin"></i></a>
    </div>
    <div class="github">
      <a href="https://github.com/Nerocodes" target="blank"><i class="fab fa-github-square"></i></a>
    </div>
    <div class="twitter">
      <a href="https://twitter.com/nerocodes" target="blank"><i class="fab fa-twitter-square"></i></a>
    </div>
    <div class="resume">
      <a href="./oghenero.pdf" target="_blank"><i class="fas fa-external-link-square-alt"></i></a>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Social'
}
</script>

<style scoped>
.socials {
  display: flex;
  justify-content: center;
  font-size: 2rem;
  color: #ffffff;
  background-color: #64766a;
  width: 100%;
  padding: 1rem 0rem;
}

.socials div {
  margin-right: 1rem;
}

.socials div:hover i{
  color: #c0a9bd;
}

.socials div:last-child {
  margin-right: 0rem;
}

a {
  color: inherit;
}
</style>