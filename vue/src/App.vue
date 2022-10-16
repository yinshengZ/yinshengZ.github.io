<template>


  <div class="container">
    <nav>
      <p>(navigation bar)</p>
    </nav>


    <div class="grid-container">
      
    <div class="grid-item">
      <div class="photo-box">
      <n-card
      hoverable>
        
          <template #cover
          >
          <img src="../src/assets/profile.png" alt="profile-photo" width="250" height="300">
        </template>
        
      
      </n-card>   
    </div> 
     


    <div class="description-box">
      <personal-experience></personal-experience>
    </div>
</div>

    <div class="personal-details">
      <div class="grid-item">
      <n-card
      hoverable>
        <div class="personal-description">
        <h1>Yinsheng Zhou</h1>
        <n-p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus sapiente deserunt sint in architecto ipsam deleniti temporibus, ad qui non illo optio iure, maxime beatae nemo recusandae sunt? Molestiae, dolorum.</n-p>
      </div>
      <div class="description-grid">
        <div class="description-grid-item description">
          <div class="description-title">
            <n-h2>Description:</n-h2>
          </div>
          
        </div>

        <div class="description-grid-item contacts">
          <div class="description-title"><n-h2>Contacts:</n-h2></div>
          
        </div>
      </div>
      </n-card>      
     
      
     
    </div>
    

    
      <div class="projects">
      
        <n-divider
        title-placement="center">
          Projects
        </n-divider>
        <n-tabs
        type="line"
        animated>
        <n-tab-pane
        name="tcmyard-manager"
        tab="TCM Yard Manager">

        <n-card
        hoverable>
        <div class="project-aim">          
          <n-divider
          title-placement="left">
          Project Aim
        </n-divider>
        <p>
          (simple project aim and description here)
        </p>         
        </div>
        </n-card>
       


         <div class="projects-grid">
          <n-card hoverable>
            <div class="project-description">
            <n-divider title-placement="left">Project Descriptions:</n-divider>
            <p>(project details such as features, progress and so on here...)</p>
          </div>


          </n-card>
          <div class="project-screenshots">
          <n-card
          hoverable>
            <div class="slides">
            <n-carousel show-arrow>
            <img src="../src/assets/1.jpg" alt="" class="carousel-img">
            <img src="../src/assets/2.jpeg" alt="" class="carousel-img">
            <img src="../src/assets/3.jpg" alt="" class="carousel-img">
            <img src="../src/assets/4.jpg" alt="" class="carousel-img">
          </n-carousel>
            <span>project project-screenshots</span>
          </div>
        </n-card>
        </div>
         
          
          
        </div>

 
          

          
        </n-tab-pane>

        <n-tab-pane
        name="ff14-static-profile"
        tab="FF14 Static Profile">
          ff14
        </n-tab-pane>

        <n-tab-pane
        name="mixed-converters"
        tab="Mixed Converters">
        Converters
        </n-tab-pane>
        </n-tabs>
      </div>
      
      </div>
</div>
    
    
</div>


 
  



</template>

<script>

import {NDivider, NTabs, NTabPane, NH2,NP, NCarousel, NCard} from 'naive-ui'
import PersonalExperience from '@/components/profile/PersonalExperience.vue'

export default {
  name: 'App',
  components: {
    PersonalExperience,
   NDivider,
   NTabs,
   NTabPane,
  NH2,
  NP,
  NCarousel,
  NCard

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
  width:95%;
  background-color:white;
  min-height: 720px;
  border-radius:10px;
  margin-left:auto;
  margin-right:auto;
  margin-top:auto;
}
nav{
  margin:auto;
  width:95%;
  min-height: 50px;
  border-radius: 10px;
  border-style: solid;
}
.grid-container{
  display:grid;
  grid-template-columns: 300px auto;
  column-gap:5px;
  padding:25px;
 
}
.grid-item{ 
 background-color:#edf2f2; 
  border-radius:10px;
  margin-top:2px;

}
.description-grid{
  display:grid;
  grid-template-columns: auto auto;
  column-gap: 5px;
  padding:25px;
}

.description-title{
  float:left;
}

.project-aim{
  width:100%;
}

.projects-grid{
  display:grid;
  grid-template-columns: 50% 50%;
  column-gap: 25px;
  margin-top:10px;

}
.carousel-img{
  width:100%;
  height:240px;
  object-fit:cover;
}

.photo-box{
  padding:10px;
}

/*
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
*/
body{
  background: rgb(51,49,77);
  background: linear-gradient(90deg, rgba(51,49,77,1) 0%, rgba(9,121,64,1) 81%, rgba(0,212,255,1) 100%);
}
</style>
