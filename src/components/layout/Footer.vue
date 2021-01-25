<template>
   <footer>
      <div id="myName">
        <a href="https://jenniferlang1921.com">Jennifer Lang Web Design</a>
      </div>
      <div id="Attribution">
        <p>Thank you to the following:</p>
        <a href="https://www.vecteezy.com/free-vector/corporate-goals">Corporate Goals Vectors by Vecteezy</a><br>
        <a href="https://youtu.be/Wy9q22isx3U">Vue JS Crash Course Youtube Traversy Media</a>
        </div>
    </footer>
</template>

<script>
export default {
  name: "Footer"
}
</script>

<style scoped>
footer {
    background: #2A0E3F;
    color: #fff;
    padding: 100px;
    font-size: 100%;
    margin-top: 5%;
    height: 200px;
    
  }
  footer a {
    color: #fff;
    text-decoration: none;
  }

  footer a:hover {
    color: #C9E9F4;
    text-decoration: underline;
  }



  #myName{
    margin-bottom: 1%;
    width: 50%;
    font-size: 100%;
    float: left;
  }

  

  #Attribution {
    color: #fff;
    width: 40%;
    float: right;
  }

  /* wide phone*/
@media screen and (max-width: 420px) and (min-width: 0px) {

  footer {
    padding: 50px;
    margin-top: 5%;
    height: 200px;
    
  }
  
    #myName{
    width: 100%;
    float: left;
  } 

  #Attribution {
    color: #fff;
    width: 100%;
    float: left;
  } 

}
  
</style>