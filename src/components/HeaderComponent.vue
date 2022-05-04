<template>

    <header id="site_header">

        <nav class="d-flex align-items-center">

            <div class="container d-flex justify-content-between align-items-center h-100">

                <SiteLogo />

                <div class="main_menu">

                    <ul class="d-flex">
                        <li v-for="item in menu" :key="item.id"><a :href="item.href">{{item.text}}</a></li>
                        <!-- <li><a href="#">characters</a></li>
                        <li><a href="#">comics</a></li>
                        <li><a href="#">movies</a></li>
                        <li><a href="#">tv</a></li>
                        <li><a href="#">games</a></li>
                        <li><a href="#">collectibes</a></li>
                        <li><a href="#">videos</a></li>
                        <li><a href="#">fans</a></li>
                        <li><a href="#">news</a></li>
                        <li><a href="#">shop</a></li> -->
                    </ul>

                </div>
                <!-- /.main_menu -->

            </div>
            <!-- /.container -->

        </nav>
          
    </header>
    <!-- /#site_header -->
    
</template>

<script>

import SiteLogo from '@/components/LogoComponent';


export default {
  name: 'HeaderComponent',
  data(){
      return {
          menu: [
              {
                  id:1,
                  href:'#',
                  text:'characters'
              },
              {
                  id:2,
                  href:'#',
                  text:'Comics'
              },
              {
                  id:3,
                  href:'#',
                  text:'movies'
              },
              {
                  id:4,
                  href:'#',
                  text:'tv'
              },
              {
                  id:5,
                  href:'#',
                  text:'games'
              },
              {
                  id:6,
                  href:'#',
                  text:'collectibes'
              },
              {
                  id:7,
                  href:'#',
                  text:'videos'
              },
              {
                  id:8,
                  href:'#',
                  text:'fans'
              },
              {
                  id:9,
                  href:'#',
                  text:'news'
              },
              {
                  id:10,
                  href:'#',
                  text:'shop'
              }
          ]
      }
  },
  
  components: {
    SiteLogo
    
  }
}

</script>

<style lang="scss" scoped>

header{

  nav{
    height: 90px;

    ul{
        
        list-style: none;

        a{
        padding: 2.5rem 1rem;
        text-decoration:none;
        text-transform: uppercase;
        color:black;
        font-weight: 600;

            &:hover {
                border-bottom: 4px solid #0282F9;
            }
        }
    }
  }

}

</style>