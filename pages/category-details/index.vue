<script>

</script>
<script setup>

</script>
<template>

        <section class="bg-[#F5F8FF] w-full p-4 md:p-12">
            <div class="container mx-auto max-w-screen-xl"><!-- container start -->
                
                    <CategoryDetailsTopSection />
                
            </div><!-- container end -->
        </section>
        <section class="bg-[#ffffff] w-full p-4 md:p-12">
            <div class="container mx-auto max-w-screen-xl"><!-- container start -->
                    
                    <CategoryDetailsPartners />

                    <CategoryDetailsSearchProduct />
                
                <!-- more text start -->

                <CategoryDetailsMoreInfo />    
                
                <!-- more text end -->

                <!-- product table start -->

                <CategoryDetailsProductTable />


                <div class="chart-wrapper">
                            <div  class="">
                           <canvas id="myChart1"></canvas>
                    </div>
                        </div>

                <!-- product table end -->

            </div><!-- container end -->
        </section>
</template>