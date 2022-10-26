<template>


  <div class="container">
    <n-card>




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

      <personal-description></personal-description>
      </n-card>      
     
      
     
    </div>
    

    
<div class="projects">
      <n-card hoverable>
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
          <n-text type="info">
            <h3>Project Aim</h3>
          </n-text>
          
        </n-divider>
        <p>
          The aim for this project is to create a management system for the TCM Yard clinic. It aims to manage patient profiles and its records and symptom histories. 
It also aims to record treatments made to each patient, there spending on each session of treatment. 
Generating digital invoice and some basic statistics such as end of month balance, income graphs are also planned 
        </p>         
        </div> <!--end of project aim class-->

      </n-card>
       


         <div class="projects-grid">
          <n-card hoverable>
            <div class="project-description">
            <n-divider title-placement="left" dashed>Project Descriptions:</n-divider>
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
      </n-card>
        
      </div><!--end of projects class-->
      
      </div>
</div>
</n-card>
    
</div>


 




</template>

<script>
import {defineComponent} from 'vue';


import {NDivider, NTabs, NTabPane,  NCarousel, NCard, NText,} from 'naive-ui'
import PersonalExperience from '@/components/profile/PersonalExperience.vue'
import PersonalDescription from '@/components/profile/PersonalDescription.vue'



export default defineComponent({
  name: 'App',
  components: {
    PersonalExperience,
    PersonalDescription,
    NDivider,
    NTabs,
    NTabPane, 
    NCarousel,
    NCard,
    NText,

 

  },
  
});
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
/*text-align: center;*/
  color: #2c3e50;
  margin-top: 20px;  
}

body{
  background-color:#029bc263
}

.container{
  width:95%;
  background-color:rgba(85, 85, 85, 0.37);
  min-height: 720px;
  border-radius:10px;
  margin:auto;
}

@media screen and (max-width: 900px) {
  

 
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

.projects{
  margin-top:1%;
}

.project-aim{
  width:100%;
  text-align: left;
  margin-left:1%;
  
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



</style>
