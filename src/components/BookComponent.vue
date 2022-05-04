<template>

    <div class="col-2">


        <div class="card py-3">

            <img :src="book.thumb" class="card-img-top no-border" :alt="book.series">
            <!-- <img :src="thumb" class="card-img-top no-border" :alt="series"> 
            vers. destructioring-->

            <div class="card-body">
                <h6 class="card-title text-left">{{book.series}}</h6>
                <!-- <h6 class="card-title text-left">{{series}}</h6> 
                vers.destructoring-->

            </div>
            <!--/.card-body -->

        </div>
        <!-- /.card -->
        
    </div>
    <!-- /.col -->
    
</template>

<script>

    export default {
        name:'BookComponent',
        component: {

        },
        props: {
            book : Object,
            /* thumb: String,
            series: String 
            
            vers.destructoring*/
        }
        
    }

</script>

<style lang="scss" scoped>

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

</style>