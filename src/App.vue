<template>
<div class="wrapper">
  <div id="nav">
  <Header />
  </div>
  <router-view />
</div>
<Footer />
</template>
<script>
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";
export default {
  components : {
    Header,
    Footer,
  }
}
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  max-width: 1024px;
  margin: 0px auto;
  position: relative;
  border: 1px solid #97979791;
  border-top:0px;
  border-bottom: 0px;
}
.wrapper{
  padding: 0 30px;
}
#nav {
  padding:30px 0;
  
}
div#collapseExample{
  z-index: 5555;
}
#nav a {
 /* font-weight: bold;*/
  color: #222222;
  text-align: left;
  font-size: 57px;
/*  width: 100%;*/
  text-decoration: none;
  border-bottom: 1px solid #c0c0c054;
  letter-spacing: 0.02em;
}
.card.card-body {
    border: 0;
    box-shadow: 0px 3px 0px 0px #6e676761;
}

#nav a.router-link-exact-active {
  color: #42b983;
}



@media (max-width: 768px) {
.row{
    display: grid;
    grid-template-columns: 61% 45%;
}
.logo {
    margin-top: 8px;
}
#nav {
  padding: 10px;
  
}
  #app{
    margin: 0px;
    width: 106%;
  }
         .artists_box:last-child{
           display: none;
       }
  .wrapper{
    padding: 0 10px;
  }
  div#collapseExample{
    top: 1%;
  }
  .searchs {
    position: absolute;
    left: 0;
}
.form-control{
  width: 91%;
}
}

</style>
