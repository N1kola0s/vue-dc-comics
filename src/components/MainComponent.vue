<template>
<main id="site_main">

      
        <div class="content_top text-white d-flex align-items-center">

            <div class="container">

                <div class="text"> -- Content goes here  -- </div>

                <div class="row">

                    <div class="col-2" v-for="(book, index) in books" :key="index">


                        <div class="card py-3">

                            <img :src="book.thumb" class="card-img-top no-border" :alt="book.series">

                            <div class="card-body">
                                <h6 class="card-title text-left">{{book.series}}</h6>
                            </div>
                            <!--/.card-body -->

                        </div>
                        <!-- /.card -->

                        <!-- <div class="card py-3">

                            <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" class="card-img-top no-border" alt="...">

                            <div class="card-body">
                                <h6 class="card-title text-left">action Comics</h6>
                            </div>
                            

                        </div>  -->
                        

                    </div>
                    <!-- /.col -->
                    
                </div>
                <!-- /.row -->

            </div>
            <!-- /.container -->

        </div>
        <!-- /.content_top -->

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
        data(){
            return{
                books:[
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                        "price": "$19.99",
                        "series": "Action Comics",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                        "price": "$3.99",
                        "series": "American Vampire 1976",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                        "price": "$16.99",
                        "series": "Aquaman",
                        "type": "graphic novel"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                        "price": "$2.99",
                        "series": "Batgirl",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                        "price": "$3.99",
                        "series": "Batman",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                        "price": "$2.99",
                        "series": "Batman Beyond",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                        "price": "$3.99",
                        "series": "Batman/Superman",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                        "price": "$4.99",
                        "series": "Batman/Superman Annual",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                        "price": "$5.99",
                        "series": "Batman: The Joker War Zone",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                        "price": "$6.99",
                        "series": "Batman: Three Jokers",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                        "price": "$4.99",
                        "series": "Batman: White Knight Presents: Harley Quinn",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                        "price": "$16.99",
                        "series": "Catwoman",
                        "type": "graphic novel"
                    }
                ]
            }
        },

        component: {


        }
    }
</script>

<style lang="scss" scoped>

    main{

        .content_top{
            
            background-color: black;
            padding:2.5rem 0;
            height: calc(100% - 125px);

            .text{
                padding:0 2.5rem;
                font-size: 1.5rem;
            }

            
                

            .card{
                padding: 1rem 0rem;
                color: #959595;
                text-transform: uppercase;
                background-color: black;


                .card-img-top{
                    object-position: top;
                    aspect-ratio: 1/1;
                    height: 200px;
                    object-fit: cover;

                    
                }

                .card-body{
                    padding: 1rem 0rem;
                }

                h6{
                    font-size:14px;
                }
            }
        
            

        }

        .content_bottom{
            padding:2.5rem 0;
            color:white;
            background-color: #0282F9 ;

             .action_image{
                height: 48px;
                width: 37px;
                margin:0 2.31rem;
            }
        }

    }

</style>
