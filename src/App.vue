<template>
  <div id="app">
     
    <img id="MountainImg" alt="man climbing mountain" src="./assets/mountain.jpg">
   
    <Header />
    <router-view/>
     <Footer />
   
  </div>
</template>

<script>
import Header from './components/layout/Header';
import Footer from './components/layout/Footer';
export default {
  name:"app",
  components: {
    Header,
    Footer
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
    font-family: Arial, Helvetica, sans-serif;
    line-height: 1.4;
    font-size: 100%;
  }
  .btn {
    display: inline-block;
    border: none;
    background: #286E8F !important;
    color: #fff;
    padding: 7px 20px;
    font-size: 100%;
    cursor: pointer;
  }
  .btn:hover {
    background: #C9E9F4 !important;
    color: #000;
  
  }

  #MountainImg {
    width: 100%;
  }

</style>