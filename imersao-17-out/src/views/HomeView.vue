<script setup lang="ts">
import Logo from "@/assets/img/logo/Frame 57.png"
import BannerImg from "../assets/img/banner/mulher.png"
import TarjaBranca from "../assets/img/banner/retanguloBranco.png"
import TarjaAmarela from "../assets/img/banner/retanguloAmarelo.png"

</script>

<template>
  <main>
    <header>
      <div class="logo">
        <img :src="Logo" alt="">
      </div>
      <nav>
      <ul>
        <li>CATALOGUE</li>
        <li>FASHION</li>
        <li>FAVORITE</li>
        <li>LIFESTYLE</li>
      </ul>
      <button class="botao">
        SIGN UP
      </button>
    </nav>
    </header>
    
    <section class="banner">
      <div class="text">
        <div class="tarja">
          <img :src="TarjaBranca" alt="">
          <img :src="TarjaAmarela" alt="">
        </div>
        <h1>LET'S<br>EXPLORE<br>UNIQUE<br>CLOTHES.</h1>
      </div>
      <div class="img">
        <img :src="BannerImg" alt="">
      </div>

    </section>
    


  </main>
</template>

<style scoped>
main  {

  width: 1290px;
  margin: 0 auto;

}


main .banner{
  margin: 30px 0 0 0;
  display: flex;
  justify-content: space-between;
  background-color: #F4F6F5;
  border-radius: 59px;
  padding: 70px 70px 0 70px;
}

main .banner .img{
  width: 55%;
}

main .banner .img img {
  width: 100%;
  
}


main .banner .text  h1{
  font-weight: 900;
  position: absolute;
  z-index: 999;
  font-size: 80px;
  margin: 0;
  padding: 0;

}

main .banner .text {
 position: relative;
}

main .banner .text .tarja {
 position: absolute;
 z-index: 0;
}

main .banner .text .tarja img:first-child {
  width: 400px;
  left: -20px;
 position: absolute;
 z-index: 0;
}
main .banner .text .tarja img:nth-child(2){
 position: absolute;
 z-index: 0;
 top: 40%;
 width: 400px;
 left: -20px;
 top: 240px;
}


main header{
  margin-top: 30px;
  display: flex;
  justify-content: space-between;
  
}

main header nav {
  display: flex;
  align-items: center;
  gap: 15px;
  
}

main header nav ul{
  padding: 0;
  display: flex;
  gap: 15px;
}


main header nav ul li{
  list-style: none;
  padding: 0;
  font-size: 20px;
}



.botao{
  background-color: black;
  color: white;
  padding: 8px 12px;
  border-radius: 6px;
  cursor: pointer;
}


</style>
