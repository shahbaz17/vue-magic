<template>
  <div class="profile">
    <img alt="Vue logo" src="../assets/logo.png" />
    <h1>Welcome {{ email }}</h1>
    <h3>
      Your Public Address is: <i>{{ publicAddress }}</i>
    </h3>
  </div>
</template>
<script>
export default {
  data() {
    return {
      email: this.$store.state.user.email,
      issuer: this.$store.state.user.issuer,
      publicAddress: this.$store.state.user.publicAddress
    }
  }
}
</script>
<style scoped>
h3 {
  margin: 20px 0 0;
}
</style>
