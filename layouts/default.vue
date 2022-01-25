<template>
  <v-app dark>
   
   
    <v-app-bar
      :clipped-left="clipped"
      fixed
      app
     
    >
     <nav>
      
       
            <span id="linknav">  <NuxtLink to="/contatti" prefetchLinks> <span id="linkcactivelass">Contattaci</span> </NuxtLink></span>
           <NuxtLink to="/" prefetchLinks style="display:flex;align-items:center;justify-content:center;"><span id="linkcactivelass">APPARTAMENTOLUXURYVACANZEMARE</span></NuxtLink>
            <span id="linknav"> <NuxtLink to="/ordina-ora" prefetchLinks><span id="linkcactivelass">Prenota</span></NuxtLink></span>
        </nav>
      <v-btn
      style="color:#fff;"
        icon
        @click.stop="rightDrawer = !rightDrawer"
      >
        <v-icon  >mdi-menu</v-icon>
      </v-btn>
    </v-app-bar>
    <v-main style="padding:15px;margin-top:60px;">
     
           <Nuxt />
     
    </v-main>
    <v-navigation-drawer
      v-model="rightDrawer"
      :right="right"
      temporary
      fixed
    >
      <v-list>
        <v-list-item @click.native="right = !right">
          <v-list-item-action>
            <v-icon light>
              mdi-repeat
            </v-icon>
          </v-list-item-action>
          <v-list-item-title> 
           
            </v-list-item-title>
         
        </v-list-item>
         <div style="height:300px;width:100%;">
           <TheNavbar/>
         </div>
      </v-list>
    </v-navigation-drawer>
   <div>
     <Fpiede/>
   </div>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Luxury Estate Roseto'
    }
  }
}
</script>
 <style >




#background{
    
    height:100vh;
}
.interni-casa{
    width:100%;
  margin:auto;
    padding:40px;
}
.sezione-vista{
   width:100%;
   display: flex;
   align-items: center;
}
.sezione-vista img{
    width:50%;
}
.sezione-vista p{
   padding: 0 40px;
   font-size: 20px;
}
.sez-video12{
    position:absolute;
    width:240px;
    height: 70px;
    z-index: 156;
    right:0;
    border-top-left-radius: 10px;
    padding:10px;
    bottom:0;
    color:#fff;
    background-color: black;
}
.carosello12{
    width:100%;
    height:100vh;
    background-color: black;
    display: flex;
    justify-content: center;
    align-items: center;
}
.titolosezione2{
    text-align: center;
    color: rgb(255, 255, 255);
    text-shadow: 1px 1px 1px black;
}
.sezione223{
  /* border:1px solid red; */
    height:100vh;
  /* display: flex;
  justify-content: center;
  align-items: center; */
    width:100%;
    background-color: black;
    /* background-image:url('img/vistaspiaggia3.jpeg') ; */
    background-repeat: no-repeat;
    background-size: cover;
    
 
}
.sezione2 video{
    margin:auto;
}
.title1 b{
    font-size: 15px;
   
}
.title1{
    /* font-family: 'Times New Roman', Times, serif; */
    font-weight: 100;
    text-shadow: 1px 1px 0px rgba(55, 66, 111, 0.172);
    text-align: center;
    color:#fff3c968;
    font-size: 40px;
    margin-top:200px;
}


*{
    margin:0;
    padding:0;
    font-family: 'Outfit', sans-serif;
    box-sizing: border-box;
}
.container{
    width:100%;
    height: 100vh;
  
   
}
nav{
    display:flex;
   
    justify-content: center;
    align-items: center;
    height:100%;
    /* position:fixed;
    top:0;
    left:0;
    right:0; */
    margin:auto;
    width:90%;
    padding:20px;
}
nav img{
    width:60%;
  
    
}
nav span{
    padding:0 60px;
    color:#fff;
    text-shadow: 1px 1px 1px rgb(0, 0, 0);
}
video{
    height: calc(100vh - 60px);
    width:100%;
    
}

#background-video {
width: 100%;
height: 100vh;
object-fit: cover;
position: relative;
left: 0;
right: 0;
top: 0;
bottom: 0;
z-index: -1;
}
#background1-video1 {
width: 100%;
height: 100vh;
object-fit: cover;
position: fixed;
left: 0;
right: 0;
top: 0;
bottom: 0;
z-index: -1;
}

/* carosello */
.page-container {
height: 100vh;
}

.title {
display: flex;
align-items: center;
justify-content: center;
height: 30vh;
}

#title-p-1 {
text-align: center;
font-size: 40px;
padding: 60px 10px 0 0;
text-shadow: 3px 4px 1px rgba(0, 0, 0, 0.2);

}

#nola {
font-size: 90px;
font-family: 'Arizonia', cursive;
transform: rotate(-10deg);
text-shadow: 3px 4px 1px rgba(0, 0, 0, 0.2);
}

.carousel-wrapper {
display: flex;
justify-content: center;
align-items: center;

width:99%;
height:75%;
}

.carousel {
height:100%;
display: flex;

align-items: center;
width: 100%;

position: relative;
}

.carousel__slide {
width: 100%;
height: 100%;
border-radius: 2px;
overflow: hidden;
box-shadow: 10px 10px 10px 1px rgba(0, 0, 0, .2);
}

.carousel__slide img {
width: 100%;
height: 100%;
object-fit: cover;
object-position: center;
}

.carousel__prev{
font-size: 20px;
padding: 5px 10px;
border:2px solid #fff;
cursor: pointer;
margin:0 20px;
color: rgb(255, 255, 255);
position:absolute;
left:0;
background-color: rgba(0, 0, 0, 0.6);
}
.carousel__next {
font-size: 20px;
background-color: rgba(0, 0, 0, 0.6);
padding: 5px 10px;
border:2px solid #fff;
cursor: pointer;
margin:0 20px;
color: rgb(255, 255, 255);
position:absolute;
right:0;
/* color: #D4AF37; */
}

.carousel__bullets {
position: absolute;
top: calc(100% + 20px);
left: 50%;
transform: translateX(-50%);
padding: 10px ;
background: rgba(0, 0, 0, 0.4);
border-radius: 30px;
display: flex;
align-items: center;
z-index: 333;
}

.carousel__bullets i {
font-size: 10px;
margin: 0 5px;

color: #fff;
cursor: pointer;
}

.carousel__bullets .active {
color: #ffd139;
}
/* carosello */
/* scroll */

/* width */
::-webkit-scrollbar {
width: 0px;
}

/* Track */
::-webkit-scrollbar-track {
box-shadow: inset 0 0 0px grey; 
border-radius: 0px;
}

/* Handle */
::-webkit-scrollbar-thumb {
background: red; 
border-radius: 0px;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
background: #b30000; 
}
@media only screen and (max-width: 920px) {
  #linknav{
    display:none;
  }
}
 </style>