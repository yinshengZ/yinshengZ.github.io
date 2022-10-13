<template>
    <div class="profile-box">
    <n-card
    title="Yinsheng Zhou">
    <template #cover>
        <img src="../../assets/profile.png" alt="profile-image">   
    </template>


    </n-card>
    
    </div>
</template>


<script>
import {NCard} from 'naive-ui'
export default{
    components:{
        NCard,
    }

}

</script>

<style scoped>
.profile-box{
    width:100%;
    min-height:200px;        
    background-color:white;
    float:left;
}
.n-card{
    max-width:300px;
    margin:auto;
}

</style>