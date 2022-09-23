<template>
<div>
  <div class="container">
    <div class="profile-box">
      <div class="photo-box">
        <profile-box></profile-box>
      </div>
      <div class="description">
        <description-box></description-box>
      </div>
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
  
  width:80%;

  margin:auto;
  margin-top:1em
}


.photo-box{
  width:100%;
  min-height:250px;
  border-style: solid;

}


.description{
  margin-top:1em;
  border-style:solid;
  border-radius:25px;
  width: 100%;
  height: 500px;
}



.projects{
  border-style:solid;
}
body{
  background:#1E90FF; 
}
</style>
