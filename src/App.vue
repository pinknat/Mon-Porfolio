<template>
  <div class="header">
    <h1>Mon portfolio</h1>
    <h2>Jane Doe</h2>
    <p>Fascinée depuis longtemps pour le monde du web, je me suis enfin lancée dans une formation pour devenir dévelopeuse web.</p>
  </div>

  <div class="address">
      <p><a href="https://www.google.fr/maps/place/12+Rue+des+Oliviers,+53200+La+Roche-Neuville/@47.8746112,-0.7520307,17z/data=!3m1!4b1!4m6!3m5!1s0x4808f12c7939a8a7:0xaefceff0de598651!8m2!3d47.8746112!4d-0.7520307" target="_blank">12 Rue des Oliviers <br> 53200 La Roche-Neuville</a></p>
      <p><a href="mailto:jane.doe@gmail.com" >jane.doe@gmail.com</a></p>           
      <p><a href="tel:0606060606" >0606060606</a></p>
  </div> 

  <menu class="Projets">
    <h3>Mes projets:</h3>
    <p><a href="https://github.com/pinknat/CV.git">Mon CV en ligne</a></p>
    <p><a href="../documents/CAHIER DES CHARGES-1.pdf">Cahier des charges</a></p>
    <p><a href="https://github.com/pinknat/DynamiserUnEspaceCommentaire.git">Dynamiser un espace commentaires</a></p>
    <p><a href="./pages/404.html">Ma page 404</a></p>
  </menu>  

</template> 

<script>
const btn=document.querySelector('.btn');
btn.addEventListener('click',() => {
  window.scrollTo({
    top:0,
    left:0,
    behavior: "smooth"
  })
})

</script>

<style>

.header {
  background-color: grey;
}

h1 {
  display:flex;
  justify-content:space-around;      
  align-items: center;
}
h2 {
  color :violet;
  display:flex;
  justify-content:space-around;      
  align-items: center;
}

.address{
    display:flex;
    align-items: center;
    justify-content:space-around;
    background-color: black;      
}

.address a{
    color:white;
    text-decoration: none;
}

.Projets li:hover{
    text-shadow:5px 5px 2px grey;
}

.Projets a{
    color:black;
}

.footer{
    display: block;
    background-color: black;
    color:#ffffff;
    text-align: center;
    padding: 20px;
  
}

.btn{
  height:100px;
  width: 100px;
  position:fixed;
  right:20px;
  bottom:20px;
  cursor: pointer;
}

body{
  margin:0;
  padding:0;
  font-family:"montserrat",sans serif;
}

.container{
  width:100%;
  position:absolute;
  top:50%;
  transform:translateY(-50%);
  text-align:center;
}

</style>