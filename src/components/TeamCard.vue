<template>
    <div>
                <div class="card text-white bg-dark">
                    <div class="d-flex justify-content-center p-2">
                        
                        <img :src="member.image" alt="foto del equipo"> 
                    </div>
                    <div class="card-body">
                        <h5 class="card-title">{{member.nombre}}</h5>
                        <p class="card-text">{{member.descripcion}}</p>
                        <small class="card-cod">{{member.rol}}</small>
                    </div>
                    <div class="card-footer bg-white">
                        <small class="text-muted"></small>
                    </div>
                </div>
            </div>
    
</template>

<script>
    export default {
        name: "TeamCard",
        props: ['member']
    }
</script>

<style scoped>

</style>
