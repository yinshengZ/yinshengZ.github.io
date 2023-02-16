<template>
    <div class="contacts-box">
        <n-card
        title="Contacts: ">
        
        <!--Email contact-->
        <n-popover
            placement="top"
            trigger="click"
           
            >
            <template #trigger>
                <n-button
            tertiary
                    circle
                    type="info">
                <template #icon>
                    <n-icon
                   ><email-icon /></n-icon>
                </template>
            </n-button>            

            </template>
            
            <span><a href="Mailto:yinshengZ@proton.me">yinshengZ@proton.me</a></span>
        </n-popover>


        <!--Mobile Contact-->
        <n-popover
        trigger="click"
        placement="top">
        
        <template #trigger>
            <n-button
            tertiary
            circle
            type="info">
            <template #icon>
                <n-icon>
                    <phone-icon></phone-icon>
                </n-icon>
            </template>
           
            </n-button>

        </template>
        <span>Mobile: 07908153858</span>
        </n-popover>

        <!--github contact-->
        <n-button
        tertiary
        circle
        type="info">
        <template #icon>
            <n-icon>
                <a href="https://github.com/yinshengZ" target="_blank"><github-icon></github-icon></a> 
            </n-icon>
        </template>
        </n-button>


        <n-popover
        placement="top"
        trigger="click"
        >


        <template #trigger>  
        <n-button
        tertiary
        circle
        type="info">
        <template
        #icon>
        <n-icon
        color="black">
            <qq-icon></qq-icon>
        </n-icon>
        </template>
        </n-button>

        </template>
        <span>297541852</span>
       

        </n-popover>
       

          
          
        </n-card>
    </div>
</template>



<script>
import {NCard, NButton, NIcon, NPopover} from "naive-ui"

import EmailIcon from "@/assets/icons/email.vue"
import PhoneIcon from "@/assets/icons/phone.vue"
import GithubIcon from "@/assets/icons/github.vue"
import QqIcon from "@/assets/icons/qq.vue"

export default{
    components:{NCard, NButton, NIcon, NPopover,EmailIcon, PhoneIcon, GithubIcon, QqIcon}
}


</script>

<style scope>
.contacts-box{
    padding-left:10px;
    padding-right:10px;
    border-radius:10px; 
    vertical-align: bottom;
}
.contact-list{
    margin:auto auto;
}
.contact-list>a>img{
    width:30px;
    height:30px;
}
.contact-list>img{
    width:20px;
    height:20px;
}
github-icon{
    color:black;
}
</style>