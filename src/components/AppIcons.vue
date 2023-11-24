<script>
    export default{
        data(){
            return{
                imgArray:[
                    {
                        title:"DIGITAL COMICS",
                        imgName:"buy-comics-digital-comics.png",
                    },
                    {
                        title:"DC MERCHANDISE",
                        imgName:"buy-comics-merchandise.png",
                    },
                    {
                        title:"SUBSCRIPTION",
                        imgName:"buy-comics-subscriptions.png",
                    },
                    {
                        title:"COMIC SHOP LOCATOR",
                        imgName:"buy-comics-shop-locator.png",
                    },
                    {
                        title:"DC POWER VISA",
                        imgName:"buy-dc-power-visa.svg",
                    },
                ]

            }
        },
        methods:{
            getImageUrl(imgName){
                return new URL(`../assets/img/${imgName}`, import.meta.url).href;
            }
        }
    }
</script>

<template>
    <section>
        <div class="container">
            <nav>
                <ul>
                    <li v-for="image in imgArray" :key="image.title">
                        <a href="">
                            <img :src="getImageUrl(image.imgName)" :alt="image.title">
                            <span>{{image.title}}</span>
                        </a>
                    </li>
                </ul>
            </nav>
        </div>
    </section>
</template>

<style  scoped lang="scss">
    @use "../style/partials/mixin" as *;
    @use "../style/partials/variables" as *;
        
    section{
        @include flex();
        height: 170px;
        background-color: $primary;

        ul{
            @include flexUl();
            list-style: none;
            gap: 4rem;

            a{
                text-decoration: none;
                color: white;

                img{
                    width: 50px;
                    vertical-align: middle;
                    margin-right: 1rem;
                }
            }
        }
    }
</style>