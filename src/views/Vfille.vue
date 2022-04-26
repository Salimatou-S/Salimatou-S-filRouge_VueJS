<template>
    <div class="vfille">
        <div class="titre">
            <h1>Robes fille</h1>
        </div>
        <div class="trait">

        </div>
    <div class="container ">    
        <div class="row">
            <Fille v-for="(fille,index) in filles" :key="index" :titre="fille.titre" :image="fille.image" :prix="fille.prix" :description="fille.description"/> 
        </div>
    </div> 
  </div>
</template>

<script>
// @ is an alias to /src
import Fille from '@/components/Fille.vue'
import axios from 'axios'


export default {
  name: 'Vfille',
  components: {
    Fille,  
    
  },
  
  data(){
        return {
            filles:[],
            errors: []
        }
  },
  // Fetches posts when the component is created.
  created() {
    axios.get(`http://localhost:8080/filles.json`)
    .then(response => {
      // JSON responses are automatically parsed.
      this.filles = response.data.filles
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


 