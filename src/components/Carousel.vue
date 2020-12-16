<template>

<div>
    <top-menu></top-menu>
        <!-- carousel -->
        <div id="carouselExampleCaptions" class="carousel slide" data-ride="carousel">
            <ol class="carousel-indicators">
                <li data-target="#carouselExampleCaptions" data-slide-to="0" class="active"></li>
                <li data-target="#carouselExampleCaptions" data-slide-to="1" class=""></li>
                <li data-target="#carouselExampleCaptions" data-slide-to="2" class=""></li>
            </ol>

            <div class="carousel-inner">
                <div class="carousel-item active">
                    <svg class="bd-placeholder-img bd-placeholder-img-lg d-block w-100" width="800" height="400" xmlns="http://www.w3.org/2000/svg"
                        preserveAspectRatio="xMidYMid slice" focusable="false" role="img" aria-label="Placeholder: First slide"><title>Placeholder</title>
                        <rect
                            width="100%" height="100%" fill="#777"></rect><text x="50%" y="50%" fill="#555" dy=".3em"></text></svg>
                    <div class="carousel-caption d-none d-md-block">
                        
                        <img
                        width="70%"
                        src="https://i.imgur.com/rtqvCwR.png" >

                        <br>
                        
                        <p>*Oferta valida hasta el 25 de diciembre del 2020.</p>
                    </div>
                </div>
                <div class="carousel-item">
                    <svg class="bd-placeholder-img bd-placeholder-img-lg d-block w-100" width="800" height="400" xmlns="http://www.w3.org/2000/svg"
                        preserveAspectRatio="xMidYMid slice" focusable="false" role="img" aria-label="Placeholder: Second slide"><title>Placeholder</title>
                        <rect
                            width="100%" height="100%" fill="#666"></rect><text x="50%" y="50%" fill="#444" dy=".3em"></text></svg>
                    <div class="carousel-caption d-none d-md-block">

                        <img
                        width="65%"
                        src="https://i.imgur.com/3KBxaaw.png" >

                        <br>
                        
                        <p>*Oferta valida hasta el 25 de diciembre del 2020.</p>
                    </div>
                </div>
                <div class="carousel-item">
                    <svg class="bd-placeholder-img bd-placeholder-img-lg d-block w-100" width="800" height="400" xmlns="http://www.w3.org/2000/svg"
                        preserveAspectRatio="xMidYMid slice" focusable="false" role="img" aria-label="Placeholder: Third slide"><title>Placeholder</title>
                       <rect
                            width="100%" height="100%" fill="#555"></rect><text x="50%" y="50%" fill="#333" dy=".3em"></text></svg>
                    <div class="carousel-caption d-none d-md-block">
                        
                        <img
                        width="60%"
                        src="https://i.imgur.com/gBZJ758.png" >

                        <br>
                        
                        <p>*Oferta valida hasta el 25 de diciembre del 2020.</p>
                    </div>
                </div>
            </div>
            <a class="carousel-control-prev" href="#carouselExampleCaptions" role="button" data-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="sr-only">Previous</span>
            </a>
            <a class="carousel-control-next" href="#carouselExampleCaptions" role="button" data-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="sr-only">Next</span>
            </a>
        </div>
</div>


</template>

<script>

import TopMenu from './TopMenu';

export default {
  name: "Carousel",
  components:{
      TopMenu
  }
};
</script>

<style scoped>
</style>
