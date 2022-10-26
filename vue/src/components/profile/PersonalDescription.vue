<template>
    <div class="personal-description-grid">
        <div class="main">
            <n-card>
                <h1>Yinsheng Zhou</h1>
                <h2>(site still under construction)</h2>
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Laudantium adipisci, aut culpa recusandae totam esse, quis itaque quaerat laboriosam ea eum dolor, minima magnam? Iusto similique nam id quia fugit?</p>
        
            </n-card>
            </div>

        <div class="description description-grid">
            <div class="profile profile-grid">
                <n-card
                title="Profile"
                :bodered="true"
                hoverable>
                    <p>profile</p>
                </n-card>
                
            </div>
            <div class="contacts contacts-grid">
                <n-card
                title="Contacts:"
                hoverable>
                    <n-list>
                        <n-list-item>
                       
                            <n-icon size="2em"
                            color="grey"
                            >
                            <div class="icon">
                                <email-round />   
                            </div>
                                                 
                        </n-icon>
                        <span class="email">
                            <a href="Mailto:yinshengZ@proton.me">  YinshengZ@proton.me</a>
                        </span>              
                       
                        </n-list-item>
                        <n-list-item>
                            
                            
                            <n-icon
                            size="2em">
                            <div class="icon">
                                
                                    <img src="@/assets/icons/github.svg" alt="Github"> 
                                </div>
                            </n-icon>
                       
                            <div class="github">
                                    <span> <a href="https://github.com/yinshengZ">Github</a> </span>
                                </div>
                        </n-list-item>
                    </n-list>
                </n-card>
                
            </div>
        </div>

    </div>
</template>


<script>

import {NCard, NList, NListItem,NIcon} from 'naive-ui'
import {EmailRound} from '@vicons/material'
export default{
    components:{
        NCard,
        NList,
        NListItem,
        NIcon,
        EmailRound
    }
}

</script>


<style scoped>


.main{
    display:grid;
}
.description{
    display:grid;
    grid-template-columns: 1fr 1fr;
}

.profile{
   text-transform: capitalize; 
}


.contact-details>a{
    text-decoration: none;
    text-emphasis-color: rgba(114, 114, 114, 0.678);
}
.contact-details>a:link{
    color:rgb(0, 0, 0);
}

.icon{
    vertical-align:middle;
    display:inline-block;
}
.icon>img{
    color:rgb(0, 255, 234);
}
.email>a{
    font-size:2em;
    text-decoration: none;
    color:rgba(71, 71, 71, 0.418)
}

</style>