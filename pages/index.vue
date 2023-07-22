<template>
  <div id="canvas">
    <div id="deep-space">

      <div class="frame1"> 
        <img src="https://www.logolynx.com/images/logolynx/7f/7fe85fb6677eaf8d18c3511c3fcaad79.png">
      </div> 

      <div class="frame">

        <div class="btn-group">
          <button class="button" type="button"><NuxtLink to="/game" style="text-decoration: none; color: inherit;"><h1>START GAME</h1></NuxtLink></button><br>
          <button class="button" type="button"><NuxtLink to="/leaderboard" style="text-decoration: none; color: inherit;"><h2>LEADER BOARD</h2></NuxtLink></button><br>
          <button class="button" type="button"><NuxtLink to="/exit" style="text-decoration: none; color: inherit;"><h1>EXIT</h1></NuxtLink></button>
        </div>    

      </div>
  </div>
  </div>
</template>

<script setup>
</script>

<style scoped>

.frame {
  width: 400px;
  height: 400px;
  margin: auto;
  text-align: center;
  border: 3px solid transparent;
  background-size: cover;
  border-radius: 30px;
  position: relative;
  top: -5rem;
  z-index: -1;
}

img {
    height: 200px;
    width: 700px;
    text-align: center;
    margin: auto;
}
.frame1 {
    text-align: center;
    margin: auto;
    z-index: 10;
    margin-top: 35px;
}

.button {
  text-align: middle;
  margin-top: 30px;
  padding-top: 10px;
  padding-bottom: 10px;
  padding-left: 80px;
  padding-right: 80px;
  background-color: transparent;
  text-shadow: #000000 0px 0px 5px, #FFF 0px 0px 10px;
  border-color: transparent;
  color: #f3f3f8;
  font-size: 16px;
}
.button:hover{
  border: 3px double #FF4294;
  border-radius: 8px;
  background-color: #ff429434;
}
.btn-group {
    margin-top: 80px;
}
</style>
