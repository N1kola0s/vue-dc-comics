<template>
<main id="site_main">

      <div class="container">
        <div class="content_top">

        </div>
        <div class="content_bottom">

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
        .content_top{
            height: 102px;
            background-color: yellow;
        }

        .content_bottom{
            height: 223px;
            background-color:orangered;
        }
    }

</style>
