<template>
   <div class="description-box">
    <n-card
    title="Personal Experiences"
    :bordered="true"
    hoverable>
      
        <p>(This is the personal experience section which should have educations, work experiences and skills here....)</p>
   

      
        <n-divider
        title-placement="left">
        Skills
        </n-divider>
        <n-list
        title="Skills"
        hoverable
        clickable>

        <n-list-item>
       
            <p>PHP/Laravel</p>
            <span>Wordpress</span>
        </n-list-item>
        <n-list-item>MySQL</n-list-item>
        <n-list-item>
            <span>Javascript/Vue</span>
        </n-list-item>
        <n-list-item>
            <span>HTML/CSS/Bootstrap</span>
        </n-list-item>
        
        </n-list>
        </n-card>
    </div>


   
    
</template>

<script>
import {NCard, NList,NListItem,NDivider} from 'naive-ui'


export default{
    components:{
        NCard,
        NList,
        NListItem,
        NDivider,
       
    }
}

</script>

<style scoped>
.description-box{
    padding-left:10px;
    padding-right:10px;
    border-radius:10px;
}



</style>