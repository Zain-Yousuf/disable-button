<template>
  <div>
    <p v-html="RowHtml"></p>
    <h3>{{ name }}</h3>
    <h3>{{ name }}</h3>
    <h3>{{ ok ? "yes" : "No" }}</h3>
    <button v-bind:disabled="disableBtn" v-on:click="updatetext">click me</button>
  </div>
</template>

<script>
export default {
  name: "home",
  data() {
    return {
      name: "zain",
      a: 10,
      b: 10,
      ok: false,
      RowHtml: "<h1>Hello zain</h1>",
      disableBtn:true
    };
  },
  methods: {
    updatetext() {
      this.name = "sufyan";
      this.ok = !this.ok;
    },
  },
};
</script>

<style lang="scss" scoped>
</style>