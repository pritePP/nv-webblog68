<template>
  <div>
    <h1>Show Users</h1>
    <p>User ID: {{ userId }}</p>
  </div>
</template>

<script>
export default {
   data () {
    return {
      userId: null
    }
  },
  created () {
    console.log("created  userId:", this.userId)
    },
     mounted () {
    this.userId = this.$route.params.userId
    console.log("created  userId:", this.userId)
    },
}
</script>

<style scoped>
/* CSS เฉพาะหน้านี้ */
</style>