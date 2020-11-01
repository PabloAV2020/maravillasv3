<template>
  <div>
      <div class="container">
        <img src="../assets/img/welcome.png" alt="Bienvenido" style="width:100%;">
        <div class="centered">
          <h1>Bienvenido a <br>
          Las Maravillas Secret Lodge Patagonia</h1>
        </div>
      </div>
      <div class="welcome">
        <div class="div1">
          <h1>Bienvenido a nuestra página oficial !</h1>
          <p> Con su excepcional belleza natural, la Patagonia siempre a atraido a amantes de la naturaleza de todo el mundo,
            un lugar donde poder ser testigos de las enormes fuerzas que gobiernan el mundo. Te queremos invitar a la Región de Aysén 
            en la Patagonia chilena, para encontrar las aventuras que siempre soñaste.  </p>
          <br>
        </div>
        <div class="div-2">
          Aquí va el reporte del clima
        </div>
      </div>
      <div class="adventure">
          <h1>Elije tu próxima aventura!</h1>
          <p> Desde nuestro Lodge puedes acceder a lugares únicos, donde podrás realizar distintas actividades como 
            pesca deportiva, senderismo, avistamiento de aves, natación, escalada, entre otros. Además podrás escoger otros 
            destinos de la región hacia donde dirigirte con comodida como las Cavernas de Marmol, Parque Nacional Queulat, 
            entre muchos otros lugares hermosos y desconocidos.  </p>
          <br>

      </div>
      <div class="row">
        <div class="column">
          <img src="../assets/img/camping.png" alt="Camping" style="width:70%">
          <p>Camping y Cabañas</p>
        </div>
        <div class="column">
          <img src="../assets/img/birdwatching.png" alt="Bird" style="width:70%">
          <p>Birdwatching</p>
        </div>
        <div class="column">
          <img src="../assets/img/fishing.png" alt="Pesca deportido" style="width:70%">
          <p>Pesca de río</p>
        </div>
        <div class="column">
          <img src="../assets/img/gastronomy.png" alt="Gastronomía" style="width:70%">
          <p>Gastronomía campestre</p>
        </div>
      </div>
      <div class="invitation">
        <p> Te invitamos a ponerte en contacto con nosotros a través de Whatsapp en el siguiente enlace para programar tu visita: </p>
      </div>
      <div class="w-button">

        <a href="https://wa.me/56974202473" target="_blank"><img src="../assets/img/wsbutton.png" width="180px"></a>

      </div>      
      <div class="adventure">
          <h1>La Experiencia de nuestros visitantes!</h1>
          <br>
      <div class="row-guests">
        <div class="column-guests">
          <img class="circular--square" src="../assets/img/cony.png" alt="Cony" >
          <br>
          <h1> Cony </h1>
          <p>"Mas fin de semanas como este por favor"</p>
        </div>
        <div class="column-guests">
          <img class="circular--square"  src="../assets/img/claudio.png" alt="Claudio" >
          <br>
          <h1> Claudio </h1>
          <p>"Excelente lugar para sacar salmones y truchas, volvería todos los años"</p>
        </div>
        <div class="column-guests">
          <img class="circular--square" src="../assets/img/karina.png" alt="Karina" >
          <br>
          <h1> Karina </h1>
          <p>"Que buena experiencia disfrutar en familia de estos paisajes y de su linda gente"</p>
        </div>
      </div>
      <div class="w-button">
        <a href="https://wa.me/56974202473" target="_blank"><img src="../assets/img/wsbutton.png" width="180px"></a>
      </div>    
      </div>
  </div>
    
    

  </div>
</template>

<script>
export default {
  name: "Home"
};

function sendWa(){
    var message = document.getElementById("message").value
    location.href = "https://wa.me/56974202473?text=" + message
}

</script>

<style scoped>


.container {
  position: relative;
  text-align: center;
}


/* Centered text */
.centered {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);

}

.centered h1 {

  font-size: 26px;
  color:#25221e;
  background-color: rgba(255, 255, 255, 0.3);
  border-radius: 25px;
  padding: 20px;
  width: 400px;
  height: 100px;

}

.welcome {
  margin:50px;
  margin-bottom:240px;
}


.div1 {
  float:left;
  width:800px;

}

.div2 {
  border-left:800px;
  float:right;
}

.div1 h1 {
  font-size: 20px;
  color: #262626;
  text-align: left;
}


.div1 p {
  font-size: 16px;
  color: #262626;
  text-align: justify;

}


.adventure{

  margin:50px;
  
}

.adventure h1{
  font-size: 20px;
  color: #262626;
  text-align: left;
}

.adventure p{
  font-size: 16px;
  color: #262626;
  text-align: justify;
}

.row {
  display: flex;
  margin:50px;
}

.column {
  flex: 25%;
  padding: 5px;
}

.row-guests {
  display: flex;
  margin:50px;
}
.column-guests{
  flex: 33%;
  padding: 5px;
}

.circular--square {
  border-radius: 50%;
  width:50%;
}

.invitation {

  text-align:left;
  margin:50px;
  font-size: 16px;
  color: #262626;

}

.column-guests h1{

  font-size:16px;
  text-align:center;

}

.column-guests p{

  font-size:14px;
  text-align:center;

}

</style>