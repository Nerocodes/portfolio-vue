<template>
  <footer>
    NeroCodes &copy; {{ year }}
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  computed: {
    year() {
      return new Date().getFullYear();
    }
  }
}
</script>