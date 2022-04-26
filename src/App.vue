<template>
  <Header/>
  
  <router-view/>

  <Footer/>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'


export default {
  components: {
    Header,
    Footer,
  },
  data() {
    return {
    }
  },
  methods: {
    
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /*text-align: center;
  color: #2c3e50;*/
}

#nav {
  padding: 0px;
  text-align: center;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: whitesmoke;
  background: #3b95ee;
  border-radius: .5rem;
}

footer a {
  font-weight: bold;
  text-decoration: none;
  color: #2c3e50;
}

footer a:hover {
  color: #3b95ee;
}

footer p {
  height: 20px;
}

</style>


<style>

/* $font1: "Saira Extra Condensed", sans-serif;
$font2: "Sofia", cursive;
$font-size: 1rem;
$font-family: "Saira Extra Condensed", sans-serif;
$color1: #bf3b40;
$color2: #080ed9;
$color3: #f9ba71;
$color4: #f7e020;
$color5: black;
$color6: #fff; */

/* body{
  height: 100vh;
} */
.rouge{
  font-family: "Saira Extra Condensed", sans-serif;
  padding-left:10px;
  color:#bf3b40;
  font-size:1.2rem ;
  padding-bottom: 0;
}
.bleu{
  color:#0066ff;
  font-family: "Sofia", cursive;
  font-weight: 100;
  font-size: 1rem;
  padding-left: 30px;
  padding-top: 0;
  padding-bottom:0;
}



.navbar2, .navbar{
  padding: 0px;
  margin-top:0 ;
}

.nav-link{
  font-family: "saira-extracondensed", sans-serif;
}
footer {
  width: 100%;
  font-family: "saira-extracondensed", sans-serif;
  font-weight: 400px;
  height: 150px;
  margin: 0;
}
.av {
  text-align: center;
  font-size: 1rem;
  margin: 0;
  padding: 5px;
  color: #fff;
  background-color: black;
}

.grid {
  display: grid;
  grid: 1fr 1fr/1fr 1fr;
  background-color: black;
  color:#fff;
  font-size: 1rem;
  text-align: center;
}

footer p a {
  color:#fff;
}

.d1,
.d2,
.d3,
.d4 {
  padding: 0 25px;
}

.bas {
  width: 23px;
  height: auto;
}

.footer-last {
  background-color: #fff;
  text-transform: uppercase;
  font-size: 0.75rem;
  margin: 5px;
  text-align: center;
  font-size: 12px;
  font-weight: 600;
}

.rezo {
  text-align: center;
  color:black;
}

i {
  margin: 0 10px 0 10px;
}

/* @media only screen and (min-width: 768px) {
 


  .grid > p {
    font-size: 1rem;
  }
}
 */

/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
} */
</style>
 -->