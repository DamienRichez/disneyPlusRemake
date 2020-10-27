<template>
  <div>
    <Navbar />
    <Jumbotron v-bind:films="films" />
  </div>
</template>

<script>
import Navbar from "./Navbar.vue"
import Jumbotron from "./Jumbotron.vue"

export default {
  name: 'Accueil',
  components:{
    Navbar,
    Jumbotron
  },
  data(){
    return{
    films:{
        roiLion:{
            name: "Le Roi Lion",
            img: require("@/assets/img/roi-lion.jpg"),
            logo: require("@/assets/img/roi-lion-logo.png")
        }
    }
}
},
}
</script>

<style scoped>

</style>
