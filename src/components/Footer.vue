<template>
    <footer>
        <div class="top">
                <div>
                    <h1>¿QUIERES VISITARNOS?</h1>
                    <p>Aquí puedes contactarnos.</p>
                    <p style="font-size:14px; color:#dd9f0d;"> Whatsapp:</p><p> +56 9 974202473</p>
                    <p style="font-size:14px; color:#dd9f0d;">Email: </p><p>maravillas.camping@gmail.com</p>
                </div>
                <div>
                    <h1>  CONÓCENOS  </h1>
                </div>
                <div>
                    <h1> SÍGUENOS </h1>
                    <a href="https://www.facebook.com/maravillas.secretlodge/" target="_blank">
                        <div class="facebook">
                                <img src="../assets/svg/fb.svg" alt="Logo" height="40" width="40" >
                        </div>
                    </a>
                    <br>
                    <a href="https://www.instagram.com/maravillas.secretlodge/" target="_blank">
                        <div class="instagram">
                                <img src="../assets/svg/ig.svg" alt="Logo" height="40" width="40" >
                        </div>
                    </a>    
                </div>
        </div>
        <div class="bottom">
            <p> © Todos los derechos reservados  - Las Maravillas Secret Lodge - 2020 </p>
            <br>
        </div>
    </footer>  
</template>


<script>
export default {
	props: ['navLinks'],
}
</script>

<style scoped>

.top{
    
    display: flex;
    justify-content: space-around;
    text-align: left;   
    }


.top h1{
    color:#c3c3c3;
    font-size: 16px;
}    

.top p{
    color:#c3c3c3;
    font-size: 14px;
} 



.bottom p{
    color:#dd9f0d;
    font-size: 14px;
    font-weight: bolder;
}

footer {
    background-color:#2c353c;
    padding: 10px;
    text-align: center;
}

.bottom a{
    color:aquamarine;


}
</style>
