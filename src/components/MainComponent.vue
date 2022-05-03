<template>
<main id="site_main">

      
        <div class="content_top text-white d-flex align-items-center">

            <div class="container">

                <div class="text"> -- Content goes here  -- </div>

            </div>

        </div>

        <div class="content_bottom">

            <div class="container h-100">

                 <div class="row align-items-center h-100">

                    <div class="col">

                        <div class="actions d-flex aling-items-center">

                            <div class="action_image d-flex align-items-center">
                                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                            </div>
                            <div class="action_text d-flex align-items-center text-uppercase">
                                digital comics
                            </div>
                        </div>
                            
                    </div>

                    <div class="col">

                        <div class="actions d-flex aling-items-center">

                            <div class="action_image d-flex align-items-center">
                                <img src="../assets/img/buy-comics-merchandise.png" alt="">
                            </div>
                            <div class="action_text d-flex align-items-center text-uppercase">
                                dc merchandise
                            </div>
                        </div>
                            
                    </div>

                    <div class="col">

                        <div class="actions d-flex aling-items-center">

                            <div class="action_image d-flex align-items-center">
                                <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                            </div>
                            <div class="action_text d-flex align-items-center text-uppercase">
                                subscription
                            </div>
                        </div>
                            
                    </div>

                    <div class="col">

                        <div class="actions d-flex aling-items-center">

                            <div class="action_image d-flex align-items-center">
                                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                            </div>
                            <div class="action_text d-flex align-items-center text-uppercase">
                                comic shop locator
                            </div>
                        </div>
                            
                    </div>

                    <div class="col">

                        <div class="actions d-flex aling-items-center">

                            <div class="action_image d-flex align-items-center">
                                <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                            </div>
                            <div class="action_text d-flex align-items-center text-uppercase">
                                dc power visa
                            </div>
                        </div>
                            
                    </div>
                    
                </div>
                
            </div>

        </div>
           
      
      
    </main>
    <!-- /#site_main -->
    
</template>

<script>
    export default {
        name:'MainComponent',
        component: {


        }
    }
</script>

<style lang="scss" scoped>

    main{
        height: calc(100vh - 180px);

        .content_top{
            
            background-color: black;
            padding:2.5rem 0;
            height: calc(100% - 125px);

            .text{
                padding:0 2.5rem;
                font-size: 1.5rem;
            }
            

        }

        .content_bottom{
            position:relative;
            z-index:1;
            padding:2.5rem 0;
            color:white;
            background-color: #0282F9 ;
            height: 125px;

             .action_image{
                height: 48px;
                width: 37px;
                margin:0 2.31rem;
            }
        }

    }

</style>
