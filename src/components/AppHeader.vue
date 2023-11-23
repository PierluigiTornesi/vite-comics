<script>
    export default{
        data(){
            return{
                navItems: [
                    {
                        title: "CHARACTERS",
                        isActive: false,
                    },
                    {
                        title: "COMICS",
                        isActive: true,
                    },
                    {
                        title: "MOVIES",
                        isActive: false,
                    },
                    {
                        title: "TV",
                        isActive: false,
                    },
                    {
                        title: "GAMES",
                        isActive: false,
                    },
                    {
                        title: "COLLECTIBLES",
                        isActive: false,
                    },
                    {
                        title: "VIDEOS",
                        isActive: false,
                    },
                    {
                        title: "FANS",
                        isActive: false,
                    },
                    {
                        title: "NEWS",
                        isActive: false,
                    },
                    {
                        title: "SHOP",
                        isActive: false,
                    },
                ]
            }
        }
    }
</script>

<template>
    <header class="container">
        <div class="logo">
            <img src="../assets/img/dc-logo.png" alt="Logo DC">
        </div>
        <nav>
            <ul>
                <li v-for="item in navItems"  :key="item.title">
                    <a :class="{'active' : item.isActive}" href="">{{item.title}}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style  scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;
    header{
        @include flexHeader();
        height: 150px;
        padding: 1rem;
        
        ul{
            @include flexUl();
            list-style: none;
            gap: 0.4rem;

            a{
                padding: 4rem 1rem;
                text-decoration: none;
                color: black;
                font-weight: bold;
                font-size: 0.9rem;
                @include border();

                &:hover{
                    color: $primary;
                    border-bottom-color: $primary;
                }

                &.active{
                    color: $primary;
                    border-bottom-color: $primary;

                }
            }
        }
    }
</style>
