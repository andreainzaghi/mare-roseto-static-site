<template>
<div>
    <ul>
        <li><NuxtLink to="/dove-siamo" prefetchLinks><p id="linkcactivelass">Dove siamo</p> </NuxtLink></li>
        <li><NuxtLink to="/interni-esterni" prefetchLinks><p id="linkcactivelass">Interno ed Esterno</p></NuxtLink></li>
        <li><NuxtLink to="/ordina-ora" prefetchLinks><p id="linkcactivelass"> Prenota</p></NuxtLink></li>
        <li><NuxtLink to="/contatti" prefetchLinks><p id="linkcactivelass">Contattaci</p></NuxtLink></li> 
    </ul>


</div>
</template>


<style >
#linkcactivelass{
 color:#fff;
   list-style: none;
   text-decoration: none;
}
   ul li{
 color:#fff;
   list-style: none;
   text-decoration: none;
}

.nuxt-link-active {
  font-weight: bold;
 
  
}
/* exact link will show the primary color for only the exact matching link */
.nuxt-link-exact-active {
  color:red;
}

</style>