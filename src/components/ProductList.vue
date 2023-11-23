<script>
    export default{
        data(){
            return{
                sectionItem:[
                    {
                        nameImg:"DIGITAL COMICS",
                        imgPath:"",
                    }
                ]
            }
        }
    }
</script>

<template>
    <main>
        <div class="container">
            <div class="content">
                <h1>Content goes here</h1>
            </div>
        </div>
    </main>
    <section>
        <div class="container">
        </div>
    </section>
</template>

<style  scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;
    
main{
    background-color: $backMain;
    color: $white;
    height: 150px;
    display: flex;
    align-items: center;
}
    
</style>