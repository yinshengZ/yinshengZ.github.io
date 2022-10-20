<template>
   <div class="description-box">
    <n-card
    title="Personal Experiences"
    :bordered="true"
    hoverable>
      
        <p>(This is the personal experience section which should have educations, work experiences and skills here....)</p>
   

        <n-tabs
        type="card"
        animated>

        <n-tab-pane
        name="skills"
        tab="Skills">        

        <n-tabs
        type="line"
        animated>
        
        <n-tab-pane
        name="backend"
        tab="Backend">        
        <n-list
        hoverable
        bordered>
            <n-list-item>
                <span>PHP/Laravel</span>
            </n-list-item>
            <n-list-item>
                <span>MYSQL</span>
            </n-list-item>
        </n-list>
        </n-tab-pane>

        <n-tab-pane
        name="frontend"
        tab="Frontend">
        <n-list
        hoverable>
            <n-list-item>
                <span>HTML</span>
            </n-list-item>
            <n-list-item>
                <span>Javascript/Vue</span>
            </n-list-item>
            <n-list-item>
                <span>CSS</span>
            </n-list-item>
            <n-list-item>
                <span>Bootstrap</span>
            </n-list-item>
            <n-list-item>
                <span>Element-UI</span>
            </n-list-item>
            <n-list-item>
                <span>Naive-UI</span>
            </n-list-item>
        </n-list>
       </n-tab-pane>

       <n-tab-pane
       name="others"
       tab="Others">
        <n-list
        hoverable>
        <n-list-item>
            <span>Wordpress</span>
        </n-list-item>
        <n-list-item>
            <span>JAVA</span>
        </n-list-item>
        
        </n-list>
       </n-tab-pane>
    
        </n-tabs>


        </n-tab-pane><!--skills panel-->

        


        <n-tab-pane
        name="education"
        tab="Education">
        <p>Educations</p>
        </n-tab-pane>

        </n-tabs>
      
      
        </n-card>
    </div>


   
    
</template>

<script>
import {NCard, NList,NListItem,NTabs,NTabPane} from 'naive-ui'


export default{
    components:{
        NCard,
        NList,
        NListItem,
        
        NTabs,
        NTabPane
       
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