<script>
    export default{
    }
</script>

<template>
    <section>
        <div class="container">
            <nav>
                <ul>
                    <li>
                        <a href="">
                            <img src="../assets/img/buy-comics-digital-comics.png" alt=" DIGITAL COMICS">
                            <span>DIGITAL COMICS</span>
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <img src="../assets/img/buy-comics-merchandise.png" alt="DC MERCHANDISE">
                            <span>DC MERCHANDISE</span>
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <img src="../assets/img/buy-comics-subscriptions.png" alt=" SUBSCRIPTION">
                            <span>SUBSCRIPTION</span>
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <img src="../assets/img/buy-comics-shop-locator.png" alt=" COMIC SHOP LOCATOR">
                            <span>COMIC SHOP LOCATOR</span>
                        </a>
                    </li>
                    <li>
                        <a href="">
                            <img src="../assets/img/buy-dc-power-visa.svg" alt=" DC POWER VISA">
                            <span> DC POWER VISA</span>
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