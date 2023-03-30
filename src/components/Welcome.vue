<template>
  <div>
    <h3>欢迎 {{ user }} 进入电商后台管理系统</h3>
  </div>
</template>

<script>
export default {
  data() {
    return {
      user: ''
    }
  },
  created() {
    this.user = sessionStorage.getItem('user')
  }
}
</script>

<style scoped></style>
