<template>
    
        <div class="card" id = "card" >
                <div class="d-flex justify-content-center p-2">

                    <img :src="service.imagen" width="150" alt="servicio imagen" >
                            
                </div>
                <div class="card-body">
                    <h5 class="card-title">{{service.titulo}}</h5>
                    <p class="card-text">{{service.descripcion}}
                    </p>
                    <ul>
                        {{service.materias}}
                    </ul>
                    <a id = "boton" href="#" class="flex btn btn-primary">Información</a>
                </div>
        </div>


</template>

<script>
export default {
  name: "Services",
  props: ['service']
};
</script>

<style>
    #card{
        height: 720px;
        width: 300px;
    }

</style>