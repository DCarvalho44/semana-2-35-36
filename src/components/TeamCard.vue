<template>


<div class="card text-white bg-dark" >
    <div class="d-flex justify-content-center p-2">
        <img :src="member.imagen"  alt="fotografia del equipo">
    </div>
        <div class="card-body">
            <h5 class="card-title">{{member.nombre}}</h5>
            <h6 class="card-subtitle mb-2 text-muted"> {{member.rol}} </h6>
            <p class="card-text">{{member.descripcion}}</p>
            <p class="card-text">{{member.edad}}</p>

        </div>
        <div class="card-footer">
                <small class="text-muted">16 de diciembre</small>
        </div>
    </div>

</template>

<script>
    export default {
        name: "TeamCard",
        props: ['member']
    }
</script>

<style>

</style>
