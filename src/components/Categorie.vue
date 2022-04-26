<template>
    <div class="cat">
        <h1 class="cat">CATEGORIES</h1>
    </div>
    <div class="categorie">
        <div class="row">
            <div class="col-lg-4 g-8" >
                <img src="../assets/fecomp10-1.jpg"  height="400"  alt="..." >
                <h5 class="text-center femme">COLLECTION FEMME</h5>
                <router-link to="/about"><p><a class="btn btn-warning" href="#" role="button">Découvrir</a></p></router-link>
            </div>
            <div class="col-lg-4 g-8" >
                <img  src="../assets/ficomp-1.jpg" height="400"   alt="..." >
                <h5 class="text-center fille">COLLECTION FILLE</h5>
                <router-link to="/vfille"><p><a class="btn btn-danger" href="#" role="button">Découvrir</a></p></router-link> 
            </div>
            <div class="col-lg-4 g-8" >
                <img src="../assets/accessoires3.jpg" height="400"   alt="..." >
                <h5 class="text-center accessoires">ACCESSOIRES</h5>
                <p><a class="btn btn-primary" href="#" role="button">Découvrir</a></p>
            </div>
        </div>
  </div>
</template>

    <style scoped>
    .cat{
      height: 100px;
     margin-top: 40px;
      
    }
    .categorie{
     margin: 40px;
     /* width: 100%;
      display: flex; */
     /*  justify-content: space-evenly; */
    }

    .femme {
      text-decoration: none;
    }
    /* .femme{
      text-decoration: none;
    } */
    .col-lg-4{
      margin-bottom: 1.5rem;
     /*  margin: 0px; */
      align-content: center;
      text-align: center; 
     
    }

    img{

      border-radius: 10px;
    }
    h5 {
      border-radius:0 50px;
      margin-bottom: 0;
      font-weight: 500;
      font-family: "Saira Extra Condensed", sans-serif;
      color: red;
      font-size: 30px;
      color: white;
      background-color: black;
      text-decoration: none;
      
    }

   

    p a{
      font-family:"Saira Extra Condensed", sans-serif ;
      font-weight: 500;
      font-size: 20px;
      color: white;
      margin-top: 0;

    }

    h4{
      font-family: "Saira Extra Condensed", sans-serif ;
      font-size: 20px;
      font-weight: 200;
    }
    .col-lg-2 p {
      margin: 0;
      /* margin-right: .4rem;
      margin-left: .4rem; */
    }
    span{
      font-family: "Saira Extra Condensed", sans-serif ;
      font-size: 16px;
      font-weight: 800;
    }

    
</style>




