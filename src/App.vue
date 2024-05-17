<template>
  <router-link to="/">Go to first page</router-link>
  <br />
  <router-link to="/second">Go to second page</router-link>
  <br />
  <router-view />
</template>

<script>

export default {
  name: 'App',
  components: {
  }
}
</script>
