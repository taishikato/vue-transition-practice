<template>
  <div id="app">
    <Modal/>
    <TransitionModal/>
  </div>
</template>

<script>
import Modal from './components/Modal'
import TransitionModal from './components/TransitionModal'

export default {
  name: 'app',
  components: {
    Modal,
    TransitionModal
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
