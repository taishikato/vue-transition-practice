<template>
<div>
  <button v-on:click="show = !show">
    Toggle
  </button>
  <transition name="fade" v-on:enter="enter" v-on:leave="leave" appear>
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
  },
  methods: {
    enter: function(el) {
        console.log('Enter!');
    },
    leave: function(el) {
      console.log('Leave!');
    }
  }
}
</script>

<style scoped>
.fade-enter-active, .fade-leave-active {
  transition: opacity .5s
}
.fade-enter, .fade-leave-to /* .fade-leave-active below version 2.1.8 */ {
  opacity: 0
}
</style>
