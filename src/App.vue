<template>
  <div>
    <el-input v-model="$store.state.count"></el-input>
    <el-button @click="handleChange">+</el-button>
  </div>
</template>

<script>
export default {
  methods: {
    handleChange() {
      this.$store.commit('increment')
    }
  },
}
</script>