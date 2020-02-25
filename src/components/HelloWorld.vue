<template>
  <div class="hello">
    <p @click="logItOut">Title: {{ title }}</p>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      title: "This is the title"
    };
  },
  methods: {
    logItOut() {
      // `this` points to the Vue instance's data option
      console.log(`This is the value of the title: ${this.title}`);
    }
  }
};
</script>
