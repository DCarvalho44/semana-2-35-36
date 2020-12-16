<template>
  <div id="app">

      <image-text> </image-text>
      <carousel> </carousel>
      <services> </services>
      
      <!-- news -->
      <div class="container-fluid">
        <div class="row mt-md-5 mt-sm-5 mt-xs-5">
       <news> </news>
        </div>
      </div>
      
      <!-- members -->
      <div class="container-fluid">
        <div class="row justify-content-center mb-5">
          <div class="col mt-5" v-for="(miembro, index) of Team" :key="index" >
            <team-card :member="miembro" > </team-card>
          </div>
        </div>
      </div>

      <footer-section> </footer-section>

  </div>
</template>

<script>

import ImageText from './components/ImageText.vue'
import Carousel from './components/Carousel.vue'
import Services from './components/Services.vue'
import FooterSection from './components/FooterSection.vue'
import TeamCard from './components/TeamCard.vue'
import News from './components/News.vue'


export default {
  name: 'App',
  components:{
    ImageText,
    Carousel,
    Services,
    FooterSection,
    TeamCard,
    News,
  },

    data() {
      return {
        Team:[
          {
          edad : 24 , 
          nombre : 'Tatiana Castillo' ,
          descripcion : 'Tecnólogo Costos y Auditoria, amante de los animales, sin experiencia en programación' ,
          rol : 'Full Stack Development' , 
          image : 'https://i.imgur.com/hhWYp55.jpeg'
        },
        {
          edad : 28 , 
          nombre : 'Juan David Cuevas Perdomo' ,
          descripcion : 'Ingeniero químico, me gusta viajar en mi motocicleta y los videojuego' ,
          rol : 'Full Stack Development' , 
          image : 'https://i.imgur.com/Xpuq2GT.jpeg'
        },
        {
          edad : 23 , 
          nombre : 'David Carvalho Saldarriaga' ,
          descripcion : 'Ingeniero Aeronautico, amante de la lectura y de un buen cafe' ,
          rol : 'Full Stack Development' , 
          image : 'https://i.imgur.com/xR2xRF4.jpeg'
        },
        {
          edad : 25 , 
          nombre : 'Lyndon Santiago Nuñez Caviche' ,
          descripcion : 'Amante de los videojuegos y la musica, entusiasta en todo lo referente a tecnologia y sistemas.' ,
          rol : 'Full Stack Development' , 
          image : 'https://i.imgur.com/kz7Qi4n.jpg'
        },
        {
          edad : 'None' , 
          nombre : '' ,
          descripcion : '' , 
          image : 'https://claroplay.com/images/carousel/noimage_poster.png?_v=1.5.99'
        },
      ]

    }

  }

}
</script>

