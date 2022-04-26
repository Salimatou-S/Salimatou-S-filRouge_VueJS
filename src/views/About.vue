<!-- <template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
</template> -->

<template>
    <div class="about">
        <div class="titre">
            <h1>Robes femmes</h1>
        </div>
        <div class="trait">

        </div>
    <div class="container ">    
        <div class="row">
            <Femme v-for="(femme,index) in femmes" :key="index" :titre="femme.titre" :image="femme.image" :prix="femme.prix" :description="femme.description"/> 
        </div>
    </div> 
  </div>
</template>

<script>
// @ is an alias to /src
import Femme from '@/components/Femme.vue'
import axios from 'axios'


export default {
  name: 'About',
  components: {
    Femme,  
    
  },
  
  data(){
        return {
            femmes:[],
            errors: []
        }
  },
  // Fetches posts when the component is created.
  created() {
    axios.get(`http://localhost:8080/femmes.json`)
    .then(response => {
      // JSON responses are automatically parsed.
      this.femmes = response.data.femmes
    })
    .catch(e => {
      this.errors.push(e)
    })
  }  
}
</script>

<style scoped>
.titre{
      height: 50px;
      margin-top: 30px;
    }

h1{
   font-size: 2rem;
}

.trait{
  height: 2px;
  background-color: black;
  width: 80%;
  margin-left: 10%;
  margin-bottom: 10px;
}
.col-lg-4 {
      
      margin-bottom: 1.5rem;
     /*  margin-right: 0px; */
      text-align: center;
      
       
        border-radius: 4px;
        overflow: hidden;
        position: relative;
        transition: 0.2s ease;
      
      
    }

    img{

      border-radius: 10px;
    }

    
    h5 {
      font-family: "Sofia", cursive;
      color: red;
      font-size: 15px;
    }

    p{
      font-family:"Saira Extra Condensed", sans-serif ;
      font-weight: 500;

    }

    span{
      font-family: "Saira Extra Condensed", sans-serif ;
      font-size: 16px;
      font-weight: 800;
    }
     .container {
      width: 100%;
      display: flex;
      justify-content: space-around;
    } 
</style>


 