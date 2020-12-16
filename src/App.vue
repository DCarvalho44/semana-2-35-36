<template>
  <div id="app">
    
    <!-- Image and text -->

    <carousel></carousel>

    <!-- services -->

    <div class="container">
      
      <div id="services" class="row justify-content-center mb-5">
        
        <div class="col-sm-6 col-xs-12 col-lg-4 mt-5" v-for="(servicio, index) of servicios" :key="index">
        
          <services v-bind:service="servicio" ></services>

          </div>

        </div>

      </div>

      <!-- news -->

    <div id="news" class="container-fluid">
        
      <news-api ></news-api>

      </div> 
      
      <!-- members -->
    
    <div id= "team" class="container-fluid">
        
        <div class="row justify-content-center mb-5">
          
          <div class="col mt-5" v-for="(item, index) of team" :key="index">
          
            <team-card v-bind:member="item"></team-card>
          
          </div> 
        
        </div>
      
      </div>

      <!-- Footer -->

    <footer class="page-footer bg-secondary text-white pt-4">
      
      <div class="container-fluid text-center text-md-left">
        
        <footer-section id="footer" ></footer-section>

      </div>

      <div class="footer-copyright text-center py-1 bg-primary">© 2020 Copyright: TuTutor
      
      </div>

    </footer>
  
  </div>
  
</template>

<script>
import FooterSection from "./components/FooterSection.vue";
import TeamCard from "./components/TeamCard.vue";
import NewsApi from "./components/NewsApi.vue";
import Carousel from "./components/Carousel.vue";
import Services from "./components/Services.vue";

export default {
  name: "App",
  components: {
    FooterSection,
    TeamCard,
    NewsApi,
    Carousel,
    Services,
  },
  data() {
    return {
      team: [
        {
          edad: "Edad: 24 años",
          nombre: "Tatiana Castillo",
          descripcion: "Tecnólogo Costos y Auditoria, amante de los animales.",
          rol: "Full Stack Development",
          imagen: "https://i.imgur.com/hhWYp55.jpeg",
        },
        {
          edad: "Edad: 28 años",
          nombre: "Juan David Cuevas Perdomo",
          descripcion:
            "Ingeniero Químico, me gusta viajar en mi motocicleta y los videojuegos.",
          rol: "Full Stack Development",
          imagen: "https://i.imgur.com/Xpuq2GT.jpeg",
        },
        {
          edad: "Edad: 23 años",
          nombre: "David Carvalho Saldarriaga",
          descripcion:
            "Ingeniero Aeronáutico, amante de la lectura y de un buen café.",
          rol: "Full Stack Development",
          imagen: "https://i.imgur.com/xR2xRF4.jpeg",
        },
      ],
      servicios: [
        {
          titulo: "Clases personalizadas",
          descripcion:
            "Te brindamos asesoría con profesionales 100% online, y personalizada, para que puedas avanzar en tu aprendizaje escolar, no dudes en agendar cita para una clase en: ",
          materias: "Matemáticas, Física, Quimica.",
          imagen: "https://i.imgur.com/6XJUwVc.png",
        },
        {
          titulo: "Asesorias en escritos",
          descripcion:
            "Somos un grupo de especialistas, los cuales te apoyamos desde el inicio hasta la presentación final de tu proyecto de grado, no te preocupes por el estilo, manejo de citas y bibliografía estamos para apoyarte. Aprende con nosotros el arte de escribir. Te ofrecemos servicios variados en la elaboración de: ",
          materias:
            "Tesis, Monografías, Artículos acádemicos, Edición de libros, Hojas de vida",
          imagen: "https://i.imgur.com/6AUBOUB.png",
        },
        {
          titulo: "Clases de programación",
          descripcion:
            "La programación es la herramienta mas importante que podrás aprender en esta nueva década, por eso te ofrecemos cursos, completos para que aprendas todo lo que necesitas saber. Contamos con tutores altamente calificados, podrás tomar las clases online en el momento que quieras, participar de foros y acercarte a la comunidad para alcanzar tus sueños. Te ofrecemos cursos desde (Beginner, Intermediate y Expert) en: ",
          materias: "Python, Java, Desarrollo web fullstack(HTML, CSS, JS)",
          imagen: "https://i.imgur.com/BJlcpoG.png",
        },
      ],
    };
  },
};
</script>

