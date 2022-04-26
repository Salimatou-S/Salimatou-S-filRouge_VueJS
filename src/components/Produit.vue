<template>

  <div class="col-lg-2" >
      <a href="#">  <img :src="require(`@/assets/${image}`)" width="200" height="300"  class="img-fluid" alt="..." bg-image hover-overlay></a>
      <h5 class="titre">{{titre}}</h5>
      <p>{{description}}</p>
      <!-- <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod. Nullam id dolor id nibh ultricies vehicula ut id elit. Morbi leo risus, porta ac consectetur ac, vestibulum at eros. Praesent commodo cursus magna.</p> -->
      <span>{{prix}}</span>
      <!-- <p><a class="btn btn-secondary" href="#" role="button">View details &raquo;</a></p> -->
  </div><!-- /.col-lg-4 -->
</template>

<script>
export default {
  name: 'Produits',
  props: {
    titre:{
      type:String, 
      default:""},
      
      image:{
      type:String, 
      default:""},

      prix:{
      type:String, 
      default:""}, 

      description:{
      type:String, 
      default:""} 
  }
}
</script>

<style>
    /* MARKETING CONTENT
    -------------------------------------------------- */
    
    /* Center align the text within the three columns below the carousel */
    .col-lg-2 {
      
      margin-bottom: 1.5rem;
     /*  margin-right: 0px; */
      text-align: center;
      
    }

    img{

      border-radius: 10px;
    }
    h5 {
      /* font-weight: 200; */
      font-family: "Sofia", cursive;
      /* font-family:"Saira Extra Condensed", sans-serif ; */
      color: red;
      font-size: 10px;
    }

    p{
      font-family:"Saira Extra Condensed", sans-serif ;
      font-weight: 500;

    }

    /* h4{
      font-family: "Saira Extra Condensed", sans-serif ;
      font-size: 20px;
      font-weight: 200;
    } 
    .col-lg-2 p {
       margin: 0; 
      margin-right: .4rem;
      margin-left: .4rem; 
    }*/
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