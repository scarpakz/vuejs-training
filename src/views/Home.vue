<template>
  <v-app>
    <Login />
  </v-app>
</template>

<script>
// @ is an alias to /src
import Login from '../components/Login'

export default {
  name: 'home',
  components: {
    Login
  }
}
</script>
