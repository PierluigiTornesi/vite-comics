<script>
    export default{
        data(){
            return{
                linkDcComics:[
                    {
                        title: "Characters",
                    },
                    {
                        title: "Comics",
                    },
                    {
                        title: "Movies",
                    },
                    {
                        title: "TV",
                    },
                    {
                        title: "Games",
                    },
                    {
                        title: "Videos",
                    },
                    {
                        title: "News",
                    },
                ],
                linkShop:[
                    {
                        title: "Shop DC",
                    },
                    {
                        title: "Shop DC Collectibles",
                    },
                ],
                linkDc:[
                    {
                        title:"Terms Of Use",
                    },
                    {
                        title:"Privacy policy(New)",
                    },
                    {
                        title:"Ad Choices",
                    },
                    {
                        title:"Advertising",
                    },
                    {
                        title:"Jobs",
                    },
                    {
                        title:"Subscriptions",
                    },
                    {
                        title:"Talent Workshops",
                    },
                    {
                        title:"CPSC Cerificates",
                    },
                    {
                        title:"Ratings",
                    },
                    {
                        title:"Shop Help",
                    },
                    {
                        title:"Contact Us",
                    },
                ],
                linkSites:[
                    {
                        title:"DC",
                    },
                    {
                        title:"MAD Magazine",
                    },
                    {
                        title:"DC Kids",
                    },
                    {
                        title:"DC Universe",
                    },
                    {
                        title:"DC Power Visa",
                    },
                ],
            }
        }
    }
</script>

<template>
  <footer>
    <div class="dc-back">
        <div class="container">
            <section class="links">
                <div class="list">
                    <div>
                        <h3>DC COMICS</h3>
                        <ul>
                            <li v-for="item in linkDcComics" :key="item.title">
                                <a href="">{{ item.title }}</a>
                            </li>
                        </ul>
                        <h3>SHOP</h3>
                        <ul>
                            <li v-for="item in linkShop" :key="item.title">
                                <a href="">{{ item.title }}</a>
                            </li>
                        </ul>
                    </div>
                    <div>
                    <h3>DC</h3>
                        <ul>
                            <li v-for="item in linkDc" :key="item.title">
                                <a href="">{{ item.title }}</a>
                            </li>
                        </ul>
                </div>
                <div>
                    <h3>SITES</h3>
                        <ul>
                            <li v-for="item in linkSites" :key="item.title">
                                <a href="">{{ item.title }}</a>
                            </li>
                        </ul>
                </div>
                </div>
            </section>
            <div class="banner">
            </div>
        </div>
    </div>
    <div class="social">
        <div class="container">
            <div class="sign">
                <button>
                    <a href="">SIGN-UP NOW!</a>
                </button>
            </div>
            <div class="socialLink">
                <h3>FOLLOW US</h3>
                <ul>
                    <li>
                        <a href="">
                            <img src="../assets/img/footer-facebook.png" alt="">
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <img src="../assets/img/footer-twitter.png" alt="">
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <img src="../assets/img/footer-youtube.png" alt="">
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <img src="../assets/img/footer-pinterest.png" alt="">
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <img src="../assets/img/footer-periscope.png" alt="">
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
  </footer>
</template>

<style  scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;
footer{
    height: calc(100vh - 470px);

    .dc-back{
        height: calc(100vh - 570px);
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;

        .container{
            @include flex();

            .links{
                width: 40%;
                .list{
                    display: flex;
                    gap: 2rem;
                    padding: 2rem;
                    align-items: left;

                    h3{
                        color: $white;
                        padding-top: 1rem;
                        padding-bottom: 1rem;
                    }

                    ul{
                        list-style: none;

                        li{
                            margin-top: 5px;
                            
                            a{
                            color: gray;
                            text-decoration: none;
                            font-size: 0.8rem;
                            }
                        }
                    }
                }
            }

            .banner{
                width: 40%;
                height: calc(100vh - 570px);
                background-image: url(../assets/img/dc-logo-bg.png);
                background-position: center;

            }
        }
    }

    .social{
        height: 100px;
        background-color: $backFooter;
        .container{
            @include flex();

            .sign{
                margin-top: 1.5rem;
                    button{
                        border: 2px solid $primary;
                        padding: 1rem;
                        background-color: $backFooter;

                        a{
                            text-decoration: none;
                            color: $white;
                            font-size: 1.2rem;
                            font-weight: bold;
                        }
                    }
            }

            .socialLink{
                @include flex();
                margin-top: 1.5rem;

                h3{
                    color: $primary;
                    margin-right: 1rem
                }
                ul{
                    @include flexUl();
                    list-style: none;
                    gap: 1rem;

                    a{
                        text-decoration: none;
                    }
                }
            }
        }
    }


}

</style>