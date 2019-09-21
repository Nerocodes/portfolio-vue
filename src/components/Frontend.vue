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
  from { transform: translateX(-1000px) }
  to { transform: translateX( 0px) }
}

.frontend {
  animation-name: slide-in-left;
  animation-duration: 2s;
}
</style>