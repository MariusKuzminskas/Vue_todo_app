<template>
  <div id="app">
    <div class="container">
      <Header />
      <router-view/>
    </div>
  </div>
</template>

<script>
import Header from './components/layout/Header'
export default {
  name: "app",
  components: {
    Header
  }
}
</script>


<style>
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
  body {
    font-family: Arial, "Helvetica Neue", Helvetica, sans-serif;
    line-height: 1.4;
  }
  .container {
    max-width: 600px;
    margin: 0 auto;
  }
  .btn {
    display: inline-block;
    border: none;
    background: #555;
    color: #fff;
    padding: 7px 20px;
    cursor: pointer;
  }
  .btn:hover {
    background-color: #666;
  }
</style>
