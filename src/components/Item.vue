<template>
  <a :href="item.url" target="_blank">
    <v-avatar
      class="logo"
      :key="item.name"
      :tile="true"
      size="100"
    >
      <img :src="item.logo" alt="avatar">
    </v-avatar>
  </a>
</template>

<script>
export default {
  name: 'Item',
  props: ['item']
}
</script>

<style scoped>
  .logo {
    margin: 15px;
  }
</style>
