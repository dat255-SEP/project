<template>
<div class="page">

  <head>
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap-theme.min.css" integrity="sha384-rHyoN1iRsVXV4nD0JutlnGaslCJuC7uwjduW9SVrLvRYooPp2bWYgmgJQIXwl/Sp" crossorigin="anonymous">
  </head>

  <div class="hero">
    <div class="hero-container">
      <img class="logo" src="../assets/tuglife-logo.png" width="30%">
    </div>
  </div>
</div>
</template>

<!-- Scripts  -->
<script>
import '../stylesheets/style.css'
export default {
  async created () {
    setTimeout(this.gotoTug, 2000)
  },
  methods: {
    async gotoTug () {
      this.$router.push({path: '/TugBoatPage', name: 'TugBoatPage'})
    }
  }
}
</script>

 CSS
<style scoped>
.hero {
  background-image: linear-gradient(rgba(0, 0, 0, 0.0), rgba(0, 0, 0, 0.0)), url("../assets/hero-image.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  height: 100vh;
  background-attachment: fixed;
}

.hero-container {
  padding-top: 200px;
}

</style>
