<template>
  <div class="home">
    <Carousel/>
    <!-- <Fefiac /> -->
    <!-- <Promo /> -->
    <Categorie/>
    
    <div class="nouveau">
        <h1>NOUVEAUTES</h1>
    </div>
    <div class="container marketing">    
        <div class="row">
           <Produit v-for="(produit,index) in produits" :key="index" :titre="produit.titre" :image="produit.image" :prix="produit.prix" :description="produit.description" /> 
        </div>
    </div>
   <!--  <img alt="Vue logo" src="../assets/logo.png" /> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    
   
  </div>
</template>

<script>
// @ is an alias to /src
/* import HelloWorld from "@/components/HelloWorld.vue"; */
/* import Promo from "@/component/Promo.vue" */
import Carousel from "@/components/Carousel.vue"
/* import Fefiac from "@/components/Fefiac.vue" */
/* import Promo from "@/components/Promo.vue" */
import Categorie from "@/components/Categorie.vue"
import Produit from '@/components/Produit.vue'
import axios from 'axios'


export default {
  name: 'Home',
  components: {
    Carousel,
    /* Fefiac, */
    /* Promo, */
    Categorie,
    Produit,
    
    
  },
  /*data(){
        return {
            details:[
                {
                  titre:'Gîte',
                  image:'gite.png',
                },
                {
                  titre:'Randonnée',
                  image:'randonnee.png',
                },
                {
                  titre:'Ski',
                  image:'ski.png',
                },
            ],
        }
    },*/
  data(){
        return {
            produits:[],
            errors: []
        }
  },
  // Fetches posts when the component is created.
  created() {
    axios.get(`http://localhost:8080/produits.json`)
    .then(response => {
      // JSON responses are automatically parsed.
      this.produits = response.data.produits
    })
    .catch(e => {
      this.errors.push(e)
    })
  }  
}
</script>

<style>

 h1{
    font-family: "Saira Extra Condensed", sans-serif;
    padding-left: 30px;
    position: absolute;
    padding-bottom: 0;
  }
.nouveau{
      height: 80px;
      margin-top: 30px;
      
      
    }
    .container {
      margin: 0;
    }

</style>