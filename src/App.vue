<template>
  <div id="app">
    <MainSideForm></MainSideForm>
    <MainForm></MainForm>
  </div>
</template>

<script>
import MainForm from './components/MainForm.vue'
import MainSideForm from './components/MainSideForm.vue'
export default {
  components: {
    'MainSideForm' : MainSideForm,
    'MainForm' : MainForm
  }
}
</script>

<style>

a{
  text-decoration: none;
}
ul{
  list-style: none;
}
</style>
