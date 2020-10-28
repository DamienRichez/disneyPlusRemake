<template>
  <div>

    <Navbar />
    <Jumbotron v-bind:films="films" />
    
    <div class="pl-3 text-reco">
      <h3>Nouveautés</h3>
    </div>
    <div class="row p-4 col-12">
      <div class=" row col-md-10">
        <Cards :key="index" v-for="(films, index) in films" :id="index" :films="films"/>
      </div>
      <div class="col-md-2">
        <Audio />
      </div>
    </div>
    

  </div>
</template>

<script>
import Navbar from "./Navbar.vue"
import Jumbotron from "./Jumbotron.vue"
import Cards from './Cards.vue'
import Audio from './Audio.vue'

export default {
  name: 'Accueil',
  components:{
    Navbar,
    Jumbotron,
    Cards,
    Audio
  },
  data(){
    return{
    films:{
        roiLion:{
            id: 1,
            name: "Le Roi Lion",
            img: require("@/assets/img/roi-lion.jpg"),
            logo: require("@/assets/img/roi-lion-logo.png")
        },
        toyStory4:{
            id: 2,
            name: "Toy Story 4",
            img: require("@/assets/img/toystory4.jpg"),
            logo: require("@/assets/img/toystory4-logo.png")
        },
        enAvant:{
            id: 3,
            name: "En Avant",
            img: require("@/assets/img/en-avant.jpg"),
            logo: require("@/assets/img/en-avant-logo.png")
        },
        malefique:{
            id: 4,
            name: "Maléfique",
            img: require("@/assets/img/malefique.jpg"),
            logo: require("@/assets/img/malefique-logo.png")
        },
        maryPoppins:{
            id: 5,
            name: "Mary Poppins Returns",
            img: require("@/assets/img/mary-poppins.jpg"),
            logo: require("@/assets/img/mary-poppins-logo.png")
        },
        peterPan:{
            id: 6,
            name: "Peter Pan",
            img: require("@/assets/img/peter-pan.jpg"),
            logo: require("@/assets/img/peter-pan-logo.png")
        },
        frozen:{
            id: 7,
            name: "La Reine des Neiges",
            img: require("@/assets/img/frozen.jpg"),
            logo: require("@/assets/img/frozen-logo.png")
        },
        bAndB:{
            id: 8,
            name: "La Belle et la Bête",
            img: require("@/assets/img/b-and-b.jpg"),
            logo: require("@/assets/img/b-and-b-logo.png")
        },
    }
}
},
}
</script>

<style scoped>

</style>
