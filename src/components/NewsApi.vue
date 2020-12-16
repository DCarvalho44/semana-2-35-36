<template>
    <div class="row mt-md-5 mt-sm-5 mt-xs-5">
            <div class="col-lg-6 col-xs-12" v-for="(science, index) of news" :key="index">
                <div class="d-flex justify-content-center align-items-center">
    
                    <div class="p-3">
                        <img :src="science.image" alt="imagen news" width="150">
                    </div>
                    
                    <div class="p-2">
                        <h5>{{science.title}}</h5>
                        <p>
                            <br>
                            {{science.description}}
                        </p>
                    </div>
    
                </div>
                <div class="d-flex container-fluid justify-content-end pb-2 mt-n2">
                    <a :href="science.url"  target="_blank" class="btn btn-outline-info">Ver más</a>
                </div>
            </div>
    
        </div>
</template>



<script>


import axios from 'axios';

export default {
    name: 'NewsApi',
    data(){
        return{

            news: null
        }
    },
    mounted(){
        axios.get('https://gnews.io/api/v4/search?q=science&max=4&lang=es&token=b13747edddcf917bbe8a4708db5dd67b')
        .then(response => {
            (this.news = response.data.articles)
        })
    }
}
</script>

<style scoped>

</style>

