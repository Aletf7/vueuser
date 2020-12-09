<template>
  <div class="home">
    <NavBar />
    <img
      class="object-contain h-48 w-full "
      alt="UR logo"
      src="../assets/logo.png"
    />
    <HelloWorld msg="Welcome to U Recommend App" />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import NavBar from "@/components/NavBar.vue";

export default {
  name: "Home",
  components: {
    NavBar,
    HelloWorld
  }
};
</script>
