<template>
  <div>
    <div id="myTopnav" class="topnav">
      <a href="#home" class="active">Home</a>
      <a href="#news">News</a>
      <a href="#contact">Contact</a>
      <a href="#about">About</a>
      <a href="javascript:void(0);" class="icon" @click="myFunction">
        <i class="fa fa-bars"></i>
      </a>
    </div>
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
      content: 'Resize the browser window to see how your content is responsive to the size of the window.',
    };
  },
  methods: {
    myFunction() {
      var x = document.getElementById("myTopnav");
      if (x.className === "topnav") {
        x.className += " responsive";
      } else {
        x.className = "topnav";
      }
    }
  }
};
</script>

<style>
.content {
  font-family: 'Tahoma', sans-serif;
}
</style>