<template>
  <div>
    <input type="text" v-model="pid" />
    <button @click="nextPage">前往</button>

    <router-link to="/products">YA</router-link>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {
      pid: "",
    };
  },
  methods: {
    nextPage() {
      this.$router.push('/products/' + this.pid)
    },
  },
};
</script>
