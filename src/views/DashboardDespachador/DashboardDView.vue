<template>

<div>
        <div class="n">

            <div class="d-flex">
                <SidebarDComponent class="c  my-2"/>  
                <div class="rout bg-white bg-opacity-75 my-2">
                    <router-view/>
                </div>          
                </div>

              

            </div>
              <FooterComponent />
</div>

</template>

<script>


import SidebarDComponent from '@/components/SidebarDComponent.vue'
import FooterComponent from '@/components/FooterComponent.vue'

export default {
    name: "DashboardDView",
    components:{
    SidebarDComponent,
    FooterComponent
}
}
</script>

<style scoped>

.n{
    background-size: cover;
    height: 100%;
    background-image: url(/src/assets/1100background.png) ;

    
}

.c{
    width: 18%;
}
.rout{
  

     width: 80%;
     margin-left:1%;
     margin-right:1%;
}
/* Dispositivos XL (pantallas de escritorio/portailes grandes, 1200px hacia arriba) */
@media only screen and (min-width: 1421px) {
    header{margin-top: 0;}
    .col-xl-1 {width: 8.33%;}
    .col-xl-2 {width: 16.66%;}
    .col-xl-3 {width: 25%;}
    .col-xl-4 {width: 33.33%;}
    .col-xl-5 {width: 41.66%;}
    .col-xl-6 {width: 50%;}
    .col-xl-7 {width: 58.33%;}
    .col-xl-8 {width: 66.66%;}
    .col-xl-9 {width: 75%;}
    .col-xl-10 {width: 83.33%;}
    .col-xl-11 {width: 91.66%;}
    .col-xl-12 {width: 100%;}
    
    .n{
        background-size: 100% 100%;
        height: 100vh;
         background-image: url(/src/assets/1100background.png)
    }

    .c{
        width: 18%;
        height: 100vh;
    }
}
</style>