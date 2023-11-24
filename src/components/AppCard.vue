<script>
    export default{
        props:{
            series: String,
            thumb: String,
            price: String,
            type:String,
        }
    }
</script>

<template>
    <div class="card">
        <img :src="thumb" :alt="series">
        <h3>{{ series }}</h3>
    </div>
</template>

<style  scoped lang="scss">
    @use "../style/partials/mixin" as *;
    @use "../style/partials/variables" as *;
        
    .card {
        height: 100%;
        
        img{
            width: 100%;
            aspect-ratio: 1;
            object-fit: cover;
            object-position: top;
        }

        h3{
            text-align: center;
            font-size: 1rem;
        }
    }
    

</style>