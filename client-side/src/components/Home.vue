<template>
  <v-layout row wrap justify-center align-center id="main">
    <v-app-bar app color="error">
      <p>asdasdasd</p>
      <v-layout row wrap justify-end>
        <v-btn> Home </v-btn>
        <v-btn @click="login()"> Login </v-btn>

        <v-btn @click="contact()"> Contact </v-btn>
      </v-layout>
    </v-app-bar>
  </v-layout>
</template>
<script>
export default {
  data() {
    return {
      hasAccount: true,
      loginData: new Object(),
      registerData: new Object(),
      users: [],
    };
  },
  mounted() {},
  methods: {
    login() {
      this.$router.push("/login");
    },
    contact() {
      this.$router.push("/contact");
    },
  },
};
</script>
<style scoped>
.main {
  min-height: 100vh;
}
</style>
