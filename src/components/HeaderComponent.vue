<template>

  <header id="site_header">

      <div class="container">

        <nav>
          <SiteLogo />

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
    height: 93px;
    background-color:red;
  }

}

</style>
