<template>
  <div id="nav">
  <nav class="navbar navbar-light bg-dark">
  <div class="container-fluid">
      <a class="navbar-brand">
          <svg class="petit" width="40" height="33" viewBox="0 0 35 28" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <ellipse cx="16.3161" cy="11.8035" rx="16.3161" ry="11.8035" fill="#F7E020"/>
                        <path d="M21.6576 14.0838L15.5427 17.0104L16.4544 18.0073L17.385 19.0249L24.6781 27L27.2331 25.7771L25.144 23.4926L26.522 22.8331L30.793 24.0734L33.7499 22.6582L31.5676 21.8515L26.6146 19.5044L27.4083 17.3032L25.452 15.1641L21.6576 14.0838Z" fill="#080ED9" stroke="black"/>
                        <path d="M5.78296 13.0488V3.08801L10.7397 5.5782L14.7327 3.08801V13.0488H12.392V6.37506L10.7397 7.57035L8.26135 6.37506V13.0488H5.78296Z" fill="#080ED9" stroke="black"/>
                        <ellipse cx="20.2058" cy="10.2099" rx="5.47312" ry="3.63567" fill="#BF3B40"/>
                        <path d="M25.6789 10.2597C25.6789 11.635 24.1377 12.7499 22.2366 12.7499C20.3356 12.7499 18.7944 11.635 18.7944 10.2597C18.7944 8.88443 20.3356 7.76953 22.2366 7.76953C24.1377 7.76953 25.6789 8.88443 25.6789 10.2597Z" fill="#F9BA71"/>
                        <path d="M25.7478 9.26367V13.248L26.8493 14.0448L28.9146 15.0409H31.8061" stroke="#BF3B40" stroke-width="10"/>
                        <rect x="20.2402" y="16.8337" width="3.44221" height="2.49019" fill="#F9BA71"/>
              </svg> 
              <span class="rouge">Mascindye'S Creations</span>  <br/>
              <span class="bleu">Style et élégance au féminin</span>
      </a>
    <div>
    <form class="d-flex">
      <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
      <button class="btn btn-outline-primary" type="submit">Search</button>
    </form>
  </div>
  <div class="icon">
      <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" fill="white" class="bi bi-person" viewBox="0 0 16 16">
  <path d="M8 8a3 3 0 1 0 0-6 3 3 0 0 0 0 6zm2-3a2 2 0 1 1-4 0 2 2 0 0 1 4 0zm4 8c0 1-1 1-1 1H3s-1 0-1-1 1-4 6-4 6 3 6 4zm-1-.004c-.001-.246-.154-.986-.832-1.664C11.516 10.68 10.289 10 8 10c-2.29 0-3.516.68-4.168 1.332-.678.678-.83 1.418-.832 1.664h10z"/>
</svg>
<svg xmlns="http://www.w3.org/2000/svg" width="20" height="20"  fill="white" class="bi bi-heart" viewBox="0 0 16 16">
  <path d="m8 2.748-.717-.737C5.6.281 2.514.878 1.4 3.053c-.523 1.023-.641 2.5.314 4.385.92 1.815 2.834 3.989 6.286 6.357 3.452-2.368 5.365-4.542 6.286-6.357.955-1.886.838-3.362.314-4.385C13.486.878 10.4.28 8.717 2.01L8 2.748zM8 15C-7.333 4.868 3.279-3.04 7.824 1.143c.06.055.119.112.176.171a3.12 3.12 0 0 1 .176-.17C12.72-3.042 23.333 4.867 8 15z"/>
</svg>
<svg xmlns="http://www.w3.org/2000/svg" width="25" height="25"  fill="white" class="bi bi-cart4" viewBox="0 0 16 16">
  <path d="M0 2.5A.5.5 0 0 1 .5 2H2a.5.5 0 0 1 .485.379L2.89 4H14.5a.5.5 0 0 1 .485.621l-1.5 6A.5.5 0 0 1 13 11H4a.5.5 0 0 1-.485-.379L1.61 3H.5a.5.5 0 0 1-.5-.5zM3.14 5l.5 2H5V5H3.14zM6 5v2h2V5H6zm3 0v2h2V5H9zm3 0v2h1.36l.5-2H12zm1.11 3H12v2h.61l.5-2zM11 8H9v2h2V8zM8 8H6v2h2V8zM5 8H3.89l.5 2H5V8zm0 5a1 1 0 1 0 0 2 1 1 0 0 0 0-2zm-2 1a2 2 0 1 1 4 0 2 2 0 0 1-4 0zm9-1a1 1 0 1 0 0 2 1 1 0 0 0 0-2zm-2 1a2 2 0 1 1 4 0 2 2 0 0 1-4 0z"/>
</svg>
  </div>
  </div>
  
  </nav>
  <nav class="navbar2 navbar-expand-lg navbar-dark" style="background-color: #bf3b40; ">
      <div class="container-fluid">
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item" >
          <router-link to="./" style="color:#f7e020">Accueil</router-link>
          <!-- <a class="nav-link active" aria-current="page" href="#" style="color:#f7e020;">Accueil</a> -->
        </li>
        <li class="nav-item">
         <!--  <a class="nav-link" href="#" style="color:#f7e020;">Vêtements femme</a> -->
          <router-link to="/about" style="color:#f7e020">Vêtements Femme</router-link>
        </li>
        <li class="nav-item">
          <!-- <a class="nav-link" href="#" style="color:#f7e020;">Vêtements fille</a> -->
          <router-link to="/vfille" style="color:#f7e020">Vêtements Fille</router-link>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#" style="color:#f7e020;">Accessoires</a>
        </li>
      </ul>
    </div>
  </div>
</nav>
</div>
</template>

<style scoped>

.nav-link {
  font-family: "saira-extracondensed", sans-serif;
}
#nav{
  position: relative;
}
.icon{
  width: 150px;
  display: flex;
  justify-content:space-between ;
}

li a{
  font-family: "saira-extracondensed", sans-serif;
}
</style>