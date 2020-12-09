<template>
  <div class="hello">
    <h1>{{ msg }}</h1>

    <p>
      Carousel to image for films
    </p>
    <Carousel />
    <h3>Your five preference</h3>
    <ul>
      <li>
        <a href="#" target="_blank" rel="noopener">Terror</a>
      </li>
      <li>
        <a href="#" target="_blank" rel="noopener">Action</a>
      </li>
      <li>
        <a href="#" target="_blank" rel="noopener">Romantic</a>
      </li>
      <li>
        <a href="#" target="_blank" rel="noopener">Comedy</a>
      </li>
      <li>
        <a href="#" target="_blank" rel="noopener">SciFy</a>
      </li>
    </ul>
    <h3>Essential Links</h3>
    <ul>
      <li>
        <a href="#" target="_blank" rel="noopener">Core Docs</a>
      </li>
      <li>
        <a href="#" target="_blank" rel="noopener">Forum</a>
      </li>
      <li>
        <a href="#" target="_blank" rel="noopener">Community Chat</a>
      </li>
      <li>
        <a href="#" target="_blank" rel="noopener">Twitter</a>
      </li>
      <li>
        <a href="#" target="_blank" rel="noopener">News</a>
      </li>
    </ul>
    <h3>For U</h3>
    <ul>
      <li>
        <a href="#" target="_blank" rel="noopener">Inside You</a>
      </li>
      <li>
        <a href="#" target="_blank" rel="noopener">U Robot</a>
      </li>
      <li>
        <a href="#" target="_blank" rel="noopener">Music and Letter</a>
      </li>
      <li>
        <a href="#" target="_blank" rel="noopener">Scary movie</a>
      </li>
      <li>
        <a href="#" target="_blank" rel="noopener">Matrix</a>
      </li>
    </ul>
  </div>
</template>

<script>
import Carousel from "@/components/Carousel.vue";

export default {
  name: "HelloWorld",
  components: {
    Carousel
  },
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
