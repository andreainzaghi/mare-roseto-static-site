<template>
<div>
     <div  class="container">
            <video  style="z-index:1;" id="background1-video1"  src="@/image/video.mp4" loop autoplay muted ></video>
             <div class="scroll-down"><i class="fas fa-chevron-circle-down" ></i></div>
           <div  style="z-index:1;" class="basso-video">
              
                 
                            <div>32m <br>
                         <b> dalla Spiaggia</b>  </div>
                       
                            <div>75m <br>
                         <b>dal Mare</b>   </div>
                       
                            <div>75m <sup>2</sup> <br>
                         <b> Superficie</b>  </div>
                         <div>Roseto degli Abruzzi<br><b>Viale Makarska 24</b></div>
                       
                            <div id="btn1"><NuxtLink to="/ordina-ora" prefetchLinks><span id="linkcactivelass">PRENOTA</span></NuxtLink></div>
                
           </div>
           
        </div>
         <div style="z-index:2;">
            <Carosel/>
         <video id="background-video" style="z-index:1;"  src="@/image/Roseto.mp4" loop autoplay muted ></video>
         <Carosel/>
         <Carosel/>
         </div>
      
          </div>
</template>

<style scoped>
.fa-chevron-circle-down{
   animation: identifier 1s linear 1s infinite alternate;
}
   
@keyframes identifier {
  0% {color:rgb(255, 255, 255);  }
  50% { color:rgba(255, 255, 255, 0.205);  transform: scale(1.06);}
  100% { color:rgb(255, 255, 255);  }
}
#btn1{
    background-color: transparent;
    border:none;
   
    border-radius: 50px;
   
    padding:8px 24px;
   
    color:#fff;
}
#btn1:hover{
    background-color: transparent;
    border:none;
  
    border-radius: 50px;
    border:2px solid #fff;
    padding:8px 24px;
   
    color:#fff;
}
.basso-video div button{
    background-color: transparent;
    border:none;
    border-radius: 50px;
    border:2px solid #fff;
    padding:8px 24px;
    color:#fff;
}
.basso-video {
    width:90%;
    height:150px;
    margin:auto;
z-index: 1;
    position:fixed;
   color:#fff;
    right:0;
    bottom:0;
    left:0;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    font-size: 24px;
}
.basso-video div b{
    font-size: 15px;
}
.scroll-down{
  z-index:1;font-size:60px;position:fixed;top:calc(70% - 30px);left:calc(50% - 30px);
}
@media only screen and (max-width: 920px) {
   .scroll-down{
  z-index:1;font-size:60px;position:fixed;top:calc(30% - 30px);left:calc(50% - 30px);
}
  .basso-video{
     display:block;
     position:relative;
     text-align: center;
  }
  .container{
     display:flex;
     align-items:center;
     justify-content: center;
  }
}
</style>