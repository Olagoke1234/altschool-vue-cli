<template>
  <div class="hello">
    <p>{{ count }}</p>
    <button @click="incrementCount">Increment</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 12,
    };
  },

  mounted() {
    this.count += 20;
  },

  methods: {
    incrementCount() {
      this.count++;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
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
