<template>
    <footer id="site_footer">

        

        <div class="footer_top">

            <div class="container">

                <div class="row">
                    <div class="col-4">
                        <div class="row my-5">
                            <div class="col">
                                <h3 class="text-uppercase text-white">
                                    dc comics
                                </h3>

                                <ul>
                                    <li>Characthers</li>
                                    <li>Comics</li>
                                    <li>Movies</li>
                                    <li>TV</li>
                                    <li>Games</li>
                                    <li>Videos</li>
                                    <li>News</li>
                                </ul>

                                <h3 class="text-uppercase text-white">shop</h3>

                                <ul>
                                    <li>Shop DC</li>
                                    <li>Shop DC Collectibles</li>
                                </ul>

                            </div>
                            <div class="col">
                                <h3 class="text-uppercase text-white">
                                    dc
                                </h3>

                                <ul>
                                    <li>Terns Of Use</li>
                                    <li>Privacy policy (New)</li>
                                    <li>Ad Choices</li>
                                    <li>Advertising</li>
                                    <li>Jobs</li>
                                    <li>Subscriptions</li>
                                    <li>Talent Workshops</li>
                                    <li>CPSC Certificates</li>
                                    <li>Ratings</li>
                                    <li>Shop Help</li>
                                    <li>Contact Us</li>
                                </ul>
                            </div>
                            <div class="col">
                                 <h3 class="text-uppercase text-white">
                                    sites
                                </h3>
                                <ul>
                                    <li>DC</li>
                                    <li>
                                        MAD Magazine
                                    </li>
                                    <li>DC Kids</li>
                                    <li>DC Universe</li>
                                    <li>DC Power Visa</li>
                                </ul>

                            </div>

                            
                        </div>
                    </div>
                    <div class="footer_logo col-8 ">
                        <!-- <img src="../assets/img/dc-logo-bg.png" alt="dc_bg_logo"> -->
                    </div>

                </div>
                <!-- /.row -->

            </div>
            <!-- /.container -->

        </div>
        <!-- /.footer_top -->
        
        <div class="footer_bottom d-flex justify-content-center">
            <div class="container">
                <div class="row align-items-center h-100">
                    <div class="col-6">
                        <button type="button" class="btn btn-outline-primary rounded-0 border-3 text-uppercase text-white">
                            sign-up now!
                        </button>
                    </div>
                    <div class="col-6">
                        <div class=" contacts d-flex justify-content-end align-items-center">
                            <h3 class="text-uppercase px-4 my-0">
                                follow us
                            </h3>
                            <div class="social_media d-flex d-flex align-items-center">
                                <div class="channel facebook">
                                    <img src="../assets/img/footer-facebook.png" alt="facebook">

                                </div>
                                <div class="channel twitter">
                                    <img src="../assets/img/footer-twitter.png" alt="twitter">

                                </div>
                                <div class="channel youtube">
                                    <img src="../assets/img/footer-youtube.png" alt="youtube">

                                </div>
                                <div class="channel pinterest">
                                    <img src="../assets/img/footer-pinterest.png" alt="pinterest">

                                </div>
                                <div class="channel periscope">
                                    <img src="../assets/img/footer-periscope.png" alt="periscope">

                                </div>

                            </div>

                        </div>

                    </div>
                </div>


            </div>

        </div>
        <!-- /.footer_bottom -->
            
        

    </footer>
    <!-- /#site_footer -->
</template>

<script>

    export default {
        name:'FooterComponent',
        component: {

        }    
    }

</script>

<style lang="scss" scoped>

footer {

    h3{
        font-size: 20px;
    }

  .footer_top{
    /* height: 298px; */
    background-image: url('../assets/img/footer-bg.jpg');
    background-size: cover;
    background-repeat: no-repeat;

     .footer_logo {
        background-image: url("../assets/img/dc-logo-bg.png");
        background-repeat: no-repeat;
        background-position: right center;
    }

     ul{
         list-style: none;
         color:#959595;
         padding: 10px 0;
     }

  }

  .footer_bottom{
    height: 90px;
    background-color: #303030;
    color: #0282F9;

    .channel{
        padding:0 8px;
        margin-left: 10px;
    }
  }

}
</style>
