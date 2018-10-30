<template>
  <body class="bg-grey-lightest bg-cover-image bg-center h-screen">
    <!-- <div style="background-image: url('@/assets/park_1920.jpg')" class="bg-auto"> -->
      <!-- <img class="bg-contain" src="@/assets/park_1920.jpg" alt=""> -->
      <login-card></login-card>
    <!-- </div> -->
  </body>
</template>

<script>
import LoginCard from "@/components/LoginCard"

export default {
  name: "home",
  components:{
    LoginCard
  }
}
</script>

<style>
/* @responsive {
  .bg-cover-image {
    background-image: url('../assets/park_1920.jpg');
  }
} */
</style>
