<template>
<main id="site_main">

        <div class="jumbotron">

        </div>
        <!-- /.jumbotron -->

      
        <div class="content_top text-white d-flex align-items-center">

            <div class="container">

                <div class="text text-uppercase bg-primary">current series</div>

                <div class="row">

                    <BookComponent :book="book" v-for="book in books" :key="book.series"/>
                    <!-- <BookComponent :thumb="book.thumb" :series="book.series" v-for="book in books" :key="book.series"/> 
                    vers.destructoring -->
                    
                </div>
                <!-- /.row -->

                <div class="load_more text-center">
                    <a href="#" class="btn btn-primary rounded-0 border-3 text-uppercase text-white px-5">
                    load more
                    </a>
                </div>
                <!-- /.load_more -->

            </div>
            <!-- /.container -->

        </div>
        <!-- /.content_top -->

        <div class="content_bottom">

            <div class="container h-100">

                 <div class="row align-items-center h-100">

                    <div class="col" v-for="item in banner" :key="item.id">

                        <div class="actions d-flex aling-items-center">

                            <div class="action_image d-flex align-items-center">
                                <img :src="item.src" :alt="item.text">
                            </div>
                            <!-- /action_image -->
                            <div class="action_text d-flex align-items-center text-uppercase">
                               {{item.text}}
                            </div>
                            <!-- /.action_text -->
                        </div>
                        <!-- /.actions -->      
                    </div>
                    <!-- /.col -->
                </div>
                <!-- /.row -->
            </div>
            <!--/.container  -->
        </div>
        <!-- /.content_bottom -->
    </main>
    <!-- /#site_main -->
    
</template>

<script>

    import BookComponent from "@/components/BookComponent.vue";
    /* importo il componente della card */

        export default {
            name:'MainComponent',

            components: {
                BookComponent,


            },
            data(){
                return {
                    books: [
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
                    ],

                    banner: [
                        {
                            id:1,
                            src:require('@/assets/img/buy-comics-digital-comics.png'),
                            text:'Digital Comics'
                        },
                        {
                            id:2,
                            src:require('@/assets/img/buy-comics-merchandise.png'),
                            text:'dc merchandise'
                        },
                        {
                            id:3,
                            src:require('@/assets/img/buy-comics-subscriptions.png'),
                            text:'subscription'
                        },
                        {
                            id:4,
                            src:require('@/assets/img/buy-comics-shop-locator.png'),
                            text:'comic shop locator'
                        },
                        {
                            id:5,
                            src:require('@/assets/img/buy-dc-power-visa.svg'),
                            text:'dc power visa'
                        }
                    ]
                }
            }
        };
</script>

<style lang="scss" scoped>

    main{

        .jumbotron{
            
                background-image: url('../assets/img/jumbotron.jpg');
                height: 315px;
                background-size: cover;
                background-repeat: no-repeat;
            }

        .content_top{
            
            background-color: black;
            padding:2.5rem 0;
            height: calc(100% - 125px);

            .container{
            
                position:relative;

                    .text{
                    padding:0.5rem 1.5rem;
                    font-size: 1.5rem; 
                    width: fit-content;
                    background-color:#0282F9;
                    position:absolute;
                    top:-70px;
                    left: 0px;
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
