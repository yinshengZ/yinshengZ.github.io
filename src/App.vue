<template>
<div>
  <div class="container">
    <div class="profile-box">
      <profile-box></profile-box>
      <description-box></description-box>

    </div>
    <div class="projects">
      <navigation-bar></navigation-bar>
    </div>
  
    
  </div>
  
</div>


</template>

<script>

import NavigationBar from './components/navigation/NavBar.vue'
import ProfileBox from './components/profile/ProfileBox.vue'
import DescriptionBox from './components/profile/DescriptionBox.vue'

export default {
  name: 'App',
  components: {
    //HelloWorld
    NavigationBar,
    ProfileBox,
    DescriptionBox
    

  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 20px;
  
  
}
.container{
  display:grid;
  grid-template-columns:auto auto auto ;
  margin:auto;
  width:80%;
  min-height:900px; 
  background:white;
  border-radius:25px;
}
.profile-box{
  
  width:fit-content;
  min-height: 900px;
  /*border-style:solid;*/
  
 

}
.projects{
  border-style:solid;
}
body{
  background:#1E90FF; 
}
</style>
