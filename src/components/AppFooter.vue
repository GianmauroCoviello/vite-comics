<!-- parte logica (javascript) -->
<script>
export default {
    
}
</script>

<!-- parte grafica (html) -->
<template lang="">
    <footer>
        <div class="container-top-footer">
            <div class="row">
                <div class="col">
                    <div class="first-list">
                        <ul>
                            <h3>DOCS</h3>
                            <li>1</li>
                            <li>1</li>
                            <li>1</li>
                            <li>1</li>
                            <li>1</li>
                            <li>1</li>
                            <li>1</li>
                        </ul>
                        <ul>
                            <h3>DOCS</h3>
                            <li>1</li>
                            <li>1</li>
                            <li>1</li>
                            
                        </ul>
                    </div>
                    <div class="second-list">
                        <ul>
                            <h3>DOCS</h3>
                            <li>1</li>
                            <li>1</li>
                            <li>1</li>
                            <li>1</li>
                            <li>1</li>
                            <li>1</li>
                            <li>1</li>
                        </ul>

                    </div>
                    <div class="third-list">
                        <ul>
                            <h3>DOCS</h3>
                            <li>1</li>
                            <li>1</li>
                            <li>1</li>
                            <li>1</li>
                            <li>1</li>
                            <li>1</li>
                            <li>1</li>
                        </ul>

                    </div>

                </div>
                
            </div>
        </div>
        <div class="container-end-footer">
            <div class="row">
                <div class="col-50">
                    button

                </div>
                <div class="col-50">
                    icons
                    
                </div>

            </div>
        </div>

    </footer>
</template>

<!-- parte style (css/scss) -->
<style lang="scss" scoped> // inserito SASS allo style e inserito anche lo scope
    .container-top-footer{
        background-image: url('../assets/img/footer-bg.jpg');
        padding: 20px 0;
        padding-bottom: 50px;


        .row{
            display: flex;
            max-width: 1170px;
            margin: 0 auto;
            display: flex;



            .col{
                display: flex;



                ul{
                    list-style-type: none;
                    padding-right: 40px;
                }
            }
        }    
        

    }

    .container-end-footer{
        background-color: gray;
        padding: 20px 0;


        .row{
            display: flex;
            max-width: 1170px;
            margin: 0 auto;
            display: flex;


            .col-50{
                width: 50%;
            }
        }
    }
    
</style>