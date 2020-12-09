<template>
  <div class="about">
    <SideBar />
    <h1>This is an Category page</h1>
  </div>
</template>
<script>
// @ is an alias to /src
import SideBar from "@/components/SideBar.vue";

export default {
  name: "Home",
  components: {
    SideBar
  }
};
</script>
