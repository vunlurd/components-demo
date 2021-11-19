<template>
  <div id="app">
    <h2>{{ header }}</h2>
    <p>{{ content }}</p>
    <hr />
    <p>Edit header: <input v-model="header" placeholder="Type new header here..." /></p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      header: 'Turbo Project Demo',
      content: 'Resize the browser window to see how your content is responsive to the size of the window.'
    }
  }
}
</script>

<style>
#app {
  font-family: 'Roboto', sans-serif;
  padding-left: 16px;
}
</style>
