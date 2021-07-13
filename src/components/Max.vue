<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>{{ now }}</p>
  </div>
</template>

<script>
export default {
  name: "Max",
  props: {
    msg: String,
  },
  data() {
    return {
      now: new Date(),
    };
  },
  methods: {
    updateDate() {
      this.now = new Date();
    },
  },
  mounted() {
    setInterval(() => {
      this.updateDate();
      console.log("Max, you are Genius!!!");
    }, 1000);
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1 {
  color: #42b983;
}

p {
  color: #2b7c58;
}

h1,
p {
  text-shadow: 1px 1px 1px rgba(0, 0, 0, 0.14), 0 2px 1px rgba(0, 0, 0, 0.12),
    0 1px 3px rgba(0, 0, 0, 0.2);
}

h1:hover,
p:hover {
  text-shadow: 1px 2px 2px rgba(0, 0, 0, 0.14), 0 3px 1px rgba(0, 0, 0, 0.12),
    0 1px 5px rgba(0, 0, 0, 0.2);
  cursor: pointer;
}

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