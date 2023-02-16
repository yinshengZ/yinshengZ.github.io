<template>
   <div class="description-box">
    <n-card
    title=""
    :bordered="true"
    hoverable>
      
       

        <n-tabs
        type="card"
        
        animated>

        <n-tab-pane
        name="skills"
        tab="Skills">        

        <n-tabs
        type="line"
        trigger="hover"
        animated>
        
        <n-tab-pane
        name="backend"
        tab="Backend">     

        <n-card>
            <n-list
            hoverable
        >
        
            <n-list-item>
                <span>PHP/Laravel</span>
            </n-list-item>
            <n-list-item>
                <span>MYSQL</span>
            </n-list-item>
        </n-list>
        </n-card>
        
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
        <n-list
        hoverable>
        <n-list-item>
            Aberystwyth University - Computer Science 
        </n-list-item>
        <n-list-item>
            Bournemouth University - Foundation Computer Science
        </n-list-item>
        <n-list-item>
            Bishop Gore School - A Levels
        </n-list-item>
        </n-list>
        </n-tab-pane>

        <n-tab-pane
        name="works"
        tab="Works">
        
        <n-tabs
        type="lines"
        trigger="hover"
        animated>
            <n-tab-pane
            name="freelance"
            tab="Freelance">

            </n-tab-pane>
            <n-tab-pane
            name="personal_projects"
            tab="Personal Projects">

            </n-tab-pane>
        </n-tabs>

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
    margin-top:5px;
}
n-list{
    background-color:black;
}



</style>