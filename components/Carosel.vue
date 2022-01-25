<template>
<div>
 
  <v-carousel
    cycle
    height="600"
    hide-delimiter-background
    show-arrows-on-hover
    style="z-index:2;"
  >
  
    <v-carousel-item
      v-for="(slide, i) in slides"
      :key="i"
    >
    <v-col col="12" style="text-align:center;text-shadow:0px 1px 1px black;font-size:20px; background-color:#1E1E1E;">Titolo</v-col>
      <v-sheet
       
        height="100%"
      >
        <v-row
          class="fill-height"
          align="center"
          justify="center"
        >
          <div class="text-h2" style=" height: 100%;  width: 100%;">
            <img :src="slide" alt="" style="  object-fit: contain;
  height: 100%;
  width: 100%;

 ">
          </div>
        </v-row>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
 
  </div>
</template>
<script>
  export default {
    data () {
      return {
        colors: [
          'indigo',
          'warning',
          'pink darken-2',
          'red lighten-1',
          'deep-purple accent-4',
        ],
        slides: [
          'https://th.bing.com/th/id/R.937f0a5865f2ce40d2ce8ae5611004de?rik=PQirUWxKYT7a%2fw&pid=ImgRaw&r=0',
          'https://raw.githubusercontent.com/andreainzaghi/books/main/img/Background%20(39).png',
          'https://media.cntraveler.com/photos/54cbfd919abb8d533165bf66/master/w_1200,c_limit/cape-view-clifton-cape-town-south-africa.jpg',
          'Fourth',
          'Fifth',
        ],
      }
    },
  }
</script>
// import axios from 'axios'
 
// export default {
//   data(){
//       return{
//           Images:[],
//           slide:0,
//           sliding:null
//       }
//   },
//   methods:{
//       onSlideStart(slide){
//           this.sliding = true
//       },
//        onSlideEnd(slide){
//           this.sliding = false
//       }
//        },
//       async asyncData(){
//           try{
//               let { data } = await axios.get('https://jsonplaceholder.typicode.com/photos')
//               return {Images : data}
//           }catch (err){
//               console.log(err)
//           }
//       }
 
// }


