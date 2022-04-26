<template>

  <div class="col-lg-4" >
      <a href="#"><img :src="require(`@/assets/${image}`)" width="300" height="400"  class="img-fluid" alt="..." bg-image hover-overlay></a>
      <h5 class="titre">{{titre}}</h5>
      <p>{{description}}</p>
      <span>{{prix}}</span>
  </div>
</template>

<script>


export default {
  name: 'Femmes',
  props: {
    titre:String,
    image:String,
    prix:String,
    description:String

  }
}
</script>

<style scoped>

.col-lg-4{

}
img:hover{
  transform: scale(1.1);
  translate: 0.6 ease;
}


</style>