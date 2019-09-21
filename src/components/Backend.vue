<template>
  <section class="backend">
    Nodejs, Adonisjs, PHP/Laravel
  </section>
</template>

<script>
export default {
  name: 'Backend'
}
</script>

<style scoped>
@keyframes slide-in-right {
  from { transform: translateX(1000px) }
  to { transform: translateX( 0px) }
}

.backend {
  animation-name: slide-in-right;
  animation-duration: 2s;
}
</style>