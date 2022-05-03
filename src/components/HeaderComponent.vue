<template>

  <header id="site_header">

      <div class="container">

        <nav class="d-flex justify-content-between align-items-center">

            <SiteLogo />
            
            <ul class="d-flex">
                <li><a href="#">character</a></li>
                <li><a href="#">comics</a></li>
                <li><a href="#">movies</a></li>
                <li><a href="#">tv</a></li>
                <li><a href="#">games</a></li>
                <li><a href="#">collectibes</a></li>
                <li><a href="#">videos</a></li>
                <li><a href="#">fans</a></li>
                <li><a href="#">news</a></li>
                <li><a href="#">shop</a></li>
            </ul>
          
        </nav>
         
      </div>

    </header>
    <!-- /#site_header -->
    
</template>

<script>

import SiteLogo from '@/components/LogoComponent';


export default {
  name: 'HeaderComponent',
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
        padding: 2.4rem 1rem;
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
