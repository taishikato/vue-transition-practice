<template>
<div>
  <button v-on:click="show = !show">
    Toggle
  </button>
  <transition name="fade">
    <p v-if="show">hello</p>
  </transition>
</div>
</template>

<script>
export default {
  name: 'Modal',
  data() {
    return {
      show: true
    }
  }
}
</script>

<style>
</style>
