<script>
export default {
    
}
</script>

<template lang="">
    <main>
        <div class="container">
            <div class="row">
                <div class="col-100">
                    <div class="content">
                        <h1>--Content goes here--</h1>
                    </div>
                </div>
            </div>
        </div>
        <div class="container-menu">
            <div class="row-menu">
                <div class="col-25">
                    1
                    
                </div>
                <div class="col-25">
                    2
                    
                </div>
                <div class="col-25">
                    3
                    
                </div>
                <div class="col-25">
                    4
                    
                </div>
                <div class="col-25">
                    5
                    
                </div>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
    .container{
        background-color: black;
        height: 100px;


        .row{
            display: flex;
            max-width: 1170px;
            margin: 0 auto;
            display: flex;
            
        


            .col-100{
                color: white;
                display: flex;
                align-items: center;
                height: 100px;
                
                
            }


        }
    

    }

    .container-menu{
        background-color: rgb(58, 101, 242);
        height: 100px;



        .row-menu{
            display: flex;
            max-width: 1170px;
            margin: 0 auto;
            display: flex;

            .col-25{
                width: calc(100%/5);

            }
        }
    
    }
</style>