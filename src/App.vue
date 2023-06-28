<script setup>
import SideBar from './components/SideBar.vue';
</script>

<template>
  <main>
    <SideBar/>
  </main>
</template>

<style scoped lang="scss">
main {
    display: flex;
    .content {
        display: flex;
        padding: 2em;
    }
}
</style>
