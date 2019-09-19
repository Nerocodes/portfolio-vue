<template>
  <section class="frontend">
    Vuejs, Reactjs, JQuery, Bootstrap, Materialize
  </section>
</template>

<script>
export default {
  name: 'Frontend'
}
</script>

<style scoped>
@keyframes slide-in-left {
  from { margin-left: -120vw }
  to { margin-left: 33.8vw }
}

.frontend {
  animation-name: slide-in-left;
  animation-duration: 2s;
}
</style>