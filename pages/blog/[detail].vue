<script setup>
const route = useRoute();

const detail = computed (() => {
    return route.params.detail.replaceAll("-", " ");
});

</script>
<script>

</script>
<style>

</style>
<template>
        <section class="bg-white w-full p-4 md:p-12">
            <div class="container mx-auto max-w-screen-xl flex-none md:flex md:flex-row"><!-- container start -->    
                <div class="main-area basis-full p-2 md:p-3 lg:p-0 md:basis-3/5 lg:w-[668px]">
                    <div class="post-detail">
                        
                        <img class="rounded-[5px] my-3" src="@/assets/img/articales/single-post/03.jpg" alt="image">
                      
                        <h1 class="font-bold text-[32px] text-[#2B313B] leading-none mb-6">{{ detail }}</h1>
                        <div class="post-info flex-none md:flex md:justify-between">
                            <span class="publish-date-time  text-[#6C7A93] font-normal text-xs">Jul 25, 2022 • Read: 5
                                min</span>

                             <span class="social-shear flex items-center">
                                 <ul class="flex flex-row justify-end">
                                    <li class="flex ml-2"> <a href="#" class=" ml-2"><span class="flex relative">
                                        <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-sky-400 opacity-75"></span><img class=" h-5 w-5" src="@/assets/img/social/facebook24.svg" alt=""> </span></a></li>
                                    <li class="flex ml-2"><a href="#" class=" ml-2"><img class="blob infinity rounded-full h-5 w-5" src="@/assets/img/social/twitter24.svg" alt=""> </a></li>
                                    <li class="flex ml-2">  <a href="#"
                                        class=" ml-2"><span class="flex relative">
                                        <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-sky-400 opacity-75"></span><img class="h-5 w-5" src="@/assets/img/social/instagram24.svg" alt=""></span> </a></li>
                                    <li class="flex ml-2"><a href="#" class=" ml-2"><img class="blob infinity rounded-full h-5 w-5" src="@/assets/img/social/youtube24.svg" alt=""> </a></li>
                                </ul>
                             </span>   
                        </div>
                        <p class="text-[#2B313B] font-normal text-xs mb-6 leading-6">On Black Friday you can go to Rowenta for various offers. Think of discounts of up to € 250 on, for example, robot vacuum cleaners, stick vacuum cleaners, air purifiers and more. If you're looking for a new vacuum cleaner, air purifier, or other household appliance, now is the time to make your purchase. </p>
                        <p>
                            Rowenta has different types of vacuum cleaners, so there is always a model that suits your household. For example, the stick vacuum cleaners are ideal for people with a large house, while the robot vacuum cleaners are perfect for people who have little time to vacuum. Even if you suffer from allergies, an air purifier is a good purchase. In short, there is something for everyone at Rowenta on Black Friday.


                            </p>
                                       
                        <div class="info-area py-4">
                            <!-- info area start -->
                            <div class="single-info">
                                <h2 class="text-[#2B313B] text-base font-bold mb-3">What is Rowenta's most popular Black Friday offer?</h2>
                                <p class="text-[#2B313B] font-normal text-xs mb-6 leading-6">TheRowenta Silence Force RO7740vacuum cleaner has been voted 'Best in the Test' by the Consumers' Association (August 2022). This vacuum cleaner is now on sale for only € 177.99 + an extra cashback of € 20.
With a range of 11 meters and a dust bag of 4.5 liters, the Rowenta Silence Force RO7455 is suitable for larger households. Thanks to the parquet brush, you don't have to worry about your wooden floor or laminate. This brush has soft, long bristles that prevent scratching or sticking to the floor.</p>

                                    <div class="more-about bg-[#F3F7FF] p-8 rounded-[10px]">
                                        <h3 class="text-[#2B313B] text-xl mb-4">Inhoud</h3>
                                        <ul class=" list-inside list-decimal">
                                            <li><a href="" class="text-[#0052FE] text-lg font-normal">Black Friday discounts up to 250 euros at Rowenta</a></li>
                                            <li><a href="" class="text-[#0052FE] text-lg font-normal">The best Black Friday promotions of 2022 from Tefal</a></li>
                                            <li><a href="" class="text-[#0052FE] text-lg font-normal">Black Friday deals at VitalFarma</a></li>
                                            <li><a href="" class="text-[#0052FE] text-lg font-normal">World Cup 2022 starts on Sunday: These are the best</a></li>
                                            <li><a href="" class="text-[#0052FE] text-lg font-normal">Option discount at Welkoop until 30 October</a></li>
                                            <li><a href="" class="text-[#0052FE] text-lg font-normal">The best 65 inch TV deals of October 2022</a></li>
                                            <li><a href="" class="text-[#0052FE] text-lg font-normal">Slow cooker: What is it and what are its benefits?</a></li>
                                            <li><a href="" class="text-[#0052FE] text-lg font-normal">Black Friday comes early: VPN offer with 59% discount at NordVPN</a></li>
                                        </ul>
                                        
                                    </div>
                                <p class="text-[#2B313B] font-normal text-xs mb-6 leading-6">Buy your favourite Tefal products now during Black Friday and benefit from attractive discounts of up to €150. Tefal is known for its high-quality cookware and appliances, so don't miss this opportunity to complement your kitchen with their latest innovations. Whether you're looking for a new pan set, fridge or kettle, Tefal offers everything you need in the kitchen at a competitive price. Be quick, because the offers are only valid for a limited time.</p>
                                    <h2 class="text-[#2B313B] text-base font-bold mb-3">What is Rowenta's most popular Black Friday offer?</h2>
                                <p class="text-[#2B313B] font-normal text-xs mb-6 leading-6">Tefal's Black Friday offers are valid until 28 November. Tefal offers discounts of up to €150 euros on hot air fryers, multicookers, grills, ironing products, pans and more. Whether you want to upgrade products in your kitchen yourself, or are looking for a nice gift for the holidays, Tefal has you covered. When you add a product to your shopping cart on tefal's official website, the discount is immediately visible and is reflected in the price of the product. Any cashback you get on products will be added to this.</p>
                            </div>
                        </div>
                    </div>  
                    <div class="bottom-part flex-none lg:flex lg:justify-between">
                            <div class="w-full lg:w-auto more-links">
                                <h5 class=" font-bold text-xs text-black mb-2">Tags</h5>
                                <div class="flex-wrap flex md:flex-none items-center">
                                    
                                                                            
                                   

                                    <a target="_blank" href=""><span class="w-fit bg-[#EBF1FF] text-[#0051FF] text-xs font-bold px-2.5 py-1.5 rounded">Black Friday</span></a>

                                                                                
                                   

                                    <a target="_blank" href=""><span class=" w-fit bg-[#EBF1FF] text-[#0051FF] text-xs font-bold px-2.5 py-1.5 rounded mx-1">Discounts</span></a>

                                        
                                </div>
                            </div>
                            <div class="w-full mt-4 lg:mt-0 lg:w-auto social-links text-left">
                                <h5 class="font-bold text-xs text-black mb-2">Share this article</h5>
                                <ul class="flex flex-row justify-start">
                                    <li class="flex mr-2"> <a href="#" class=" mr-2"><span class="flex relative">
                                        <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-sky-400 opacity-75"></span><img class=" h-5 w-5" src="@/assets/img/social/facebook24.svg" alt=""> </span></a></li>
                                    <li class="flex mr-2"><a href="#" class=" mr-2"><img class="blob infinity rounded-full h-5 w-5" src="@/assets/img/social/twitter24.svg" alt=""> </a></li>
                                    <li class="flex mr-2">  <a href="#"
                                        class=" mr-2"><span class="flex relative">
                                        <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-sky-400 opacity-75"></span><img class="h-5 w-5" src="@/assets/img/social/instagram24.svg" alt=""></span> </a></li>
                                    <li class="flex mr-2"><a href="#" class=" mr-2"><img class="blob infinity rounded-full h-5 w-5" src="@/assets/img/social/youtube24.svg" alt=""> </a></li>
                                </ul>
                            </div>
                        </div> 
                </div>
                <div class="side-bar basis-full md:basis-2/5 lg:w-[392px]">
                    <div class="inner-area ml-0 lg:ml-4 p-2 md:p-0">
                        <div class="accordion mb-3">
                                                  
                        </div>
                        <div class="articles mb-3 border-l border-t rounded-t-[5px] border-r border-[#F5F8FF]">
                            <h3 class="p-6 border-t border-b border-[#F5F8FF] mx-auto md:text-base lg:text-2xl text-xl text-[#2B313B] font-bold">
                                Hot News</h3>
                            <a href="#" class="flex px-3 items-center justify-between align-middle transition-all opacity-100 border-b border-[#F5F8FF] hover:opacity-90 bg-white py-2.5">
                                <span class="fixed-size overflow-hidden w-[97px] h-[78px] rounded-[5px] ">
                                     <img class="object-cover mt-2 w-auto h-auto mb-0" src="@/assets/img/news/05.jpg" alt="icon">
                                </span>
                                <div class="ml-3 text-sm sm:text-xs lg:text-sm w-10/12 font-bold flex items-start flex-col">
                                   <div class="block"> Black Friday discounts up to 250 euros at Rowenta</div>
                                    
                                <div class="flex items-center justify-between mt-2 w-full">    
                                        <div class="news-tags"> 
                                            <span class="w-fit bg-[#EBF1FF] text-[#0051FF] text-xs font-semibold mr-1 px-2.5 py-1.5 rounded ">Gadget & Tablet</span>
                                        </div>
                                        
                                        <div class="post-date text-xs font-normal text-[#6C7A93] flex flex-row items-center"><svg class="ml-4 mr-1" width="10" height="10" viewBox="0 0 10 10" fill="none" xmlns="http://www.w3.org/2000/svg">
                                            <path fill-rule="evenodd" clip-rule="evenodd" d="M5 9C7.20914 9 9 7.20914 9 5C9 2.79086 7.20914 1 5 1C2.79086 1 1 2.79086 1 5C1 7.20914 2.79086 9 5 9ZM5.5 3C5.5 2.72386 5.27614 2.5 5 2.5C4.72386 2.5 4.5 2.72386 4.5 3V5C4.5 5.13261 4.55268 5.25979 4.64645 5.35355L6.06066 6.76777C6.25592 6.96303 6.5725 6.96303 6.76777 6.76777C6.96303 6.5725 6.96303 6.25592 6.76777 6.06066L5.5 4.79289V3Z" fill="white"/>
                                            </svg> 10 minutes
                                        </div>
                                    </div>
                                </div>
                            </a>
                            <a href="#" class="flex px-3 items-center justify-between align-middle transition-all opacity-100 border-b border-[#F5F8FF] hover:opacity-90 bg-white py-2.5">
                                <span class="fixed-size overflow-hidden w-[97px] h-[78px] rounded-[5px] ">
                                     <img class="object-cover mt-2 w-auto h-auto mb-0" src="@/assets/img/news/06.jpg" alt="icon">
                                </span>
                                <div class="ml-3 text-sm sm:text-xs lg:text-sm w-10/12 font-bold flex items-start flex-col">
                                   <div class="block"> Black Friday discounts up to 250 euros at Rowenta</div>
                                    
                                <div class="flex items-center justify-between mt-2 w-full">    
                                        <div class="news-tags"> 
                                            <span class="w-fit bg-[#EBF1FF] text-[#0051FF] text-xs font-semibold mr-1 px-2.5 py-1.5 rounded ">Gadget & Tablet</span>
                                        </div>
                                        
                                        <div class="post-date text-xs font-normal text-[#6C7A93] flex flex-row items-center"><svg class="ml-4 mr-1" width="10" height="10" viewBox="0 0 10 10" fill="none" xmlns="http://www.w3.org/2000/svg">
                                            <path fill-rule="evenodd" clip-rule="evenodd" d="M5 9C7.20914 9 9 7.20914 9 5C9 2.79086 7.20914 1 5 1C2.79086 1 1 2.79086 1 5C1 7.20914 2.79086 9 5 9ZM5.5 3C5.5 2.72386 5.27614 2.5 5 2.5C4.72386 2.5 4.5 2.72386 4.5 3V5C4.5 5.13261 4.55268 5.25979 4.64645 5.35355L6.06066 6.76777C6.25592 6.96303 6.5725 6.96303 6.76777 6.76777C6.96303 6.5725 6.96303 6.25592 6.76777 6.06066L5.5 4.79289V3Z" fill="white"/>
                                            </svg> 10 minutes
                                        </div>
                                    </div>
                                </div>
                            </a>
                            <a href="#" class="flex px-3 items-center justify-between align-middle transition-all opacity-100 border-b border-[#F5F8FF] hover:opacity-90 bg-white py-2.5">
                                <span class="fixed-size overflow-hidden w-[97px] h-[78px] rounded-[5px] ">
                                     <img class="object-cover mt-2 w-auto h-auto mb-0" src="@/assets/img/news/07.jpg" alt="icon">
                                </span>
                                <div class="ml-3 text-sm sm:text-xs lg:text-sm w-10/12 font-bold flex items-start flex-col">
                                   <div class="block"> Black Friday discounts up to 250 euros at Rowenta</div>
                                    
                                <div class="flex items-center justify-between mt-2 w-full">    
                                        <div class="news-tags"> 
                                            <span class="w-fit bg-[#EBF1FF] text-[#0051FF] text-xs font-semibold mr-1 px-2.5 py-1.5 rounded ">Gadget & Tablet</span>
                                        </div>
                                        
                                        <div class="post-date text-xs font-normal text-[#6C7A93] flex flex-row items-center"><svg class="ml-4 mr-1" width="10" height="10" viewBox="0 0 10 10" fill="none" xmlns="http://www.w3.org/2000/svg">
                                            <path fill-rule="evenodd" clip-rule="evenodd" d="M5 9C7.20914 9 9 7.20914 9 5C9 2.79086 7.20914 1 5 1C2.79086 1 1 2.79086 1 5C1 7.20914 2.79086 9 5 9ZM5.5 3C5.5 2.72386 5.27614 2.5 5 2.5C4.72386 2.5 4.5 2.72386 4.5 3V5C4.5 5.13261 4.55268 5.25979 4.64645 5.35355L6.06066 6.76777C6.25592 6.96303 6.5725 6.96303 6.76777 6.76777C6.96303 6.5725 6.96303 6.25592 6.76777 6.06066L5.5 4.79289V3Z" fill="white"/>
                                            </svg> 10 minutes
                                        </div>
                                    </div>
                                </div>
                            </a>
                            <a href="#" class="flex px-3 items-center justify-between align-middle transition-all opacity-100 border-b border-[#F5F8FF] hover:opacity-90 bg-white py-2.5">
                                <span class="fixed-size overflow-hidden w-[97px] h-[78px] rounded-[5px] ">
                                     <img class="object-cover mt-2 w-auto h-auto mb-0" src="@/assets/img/news/08.jpg" alt="icon">
                                </span>
                                <div class="ml-3 text-sm sm:text-xs lg:text-sm w-10/12 font-bold flex items-start flex-col">
                                   <div class="block"> Black Friday discounts up to 250 euros at Rowenta</div>
                                    
                                <div class="flex items-center justify-between mt-2 w-full">    
                                        <div class="news-tags"> 
                                            <span class="w-auto bg-[#EBF1FF] text-[#0051FF] text-xs font-semibold mr-1 px-2.5 py-1.5 rounded whitespace-nowrap ">Gadget & Tablet</span>
                                        </div>
                                        
                                        <div class="post-date text-xs font-normal text-[#6C7A93] flex flex-row items-center"><svg class="ml-4 mr-1" width="10" height="10" viewBox="0 0 10 10" fill="none" xmlns="http://www.w3.org/2000/svg">
                                            <path fill-rule="evenodd" clip-rule="evenodd" d="M5 9C7.20914 9 9 7.20914 9 5C9 2.79086 7.20914 1 5 1C2.79086 1 1 2.79086 1 5C1 7.20914 2.79086 9 5 9ZM5.5 3C5.5 2.72386 5.27614 2.5 5 2.5C4.72386 2.5 4.5 2.72386 4.5 3V5C4.5 5.13261 4.55268 5.25979 4.64645 5.35355L6.06066 6.76777C6.25592 6.96303 6.5725 6.96303 6.76777 6.76777C6.96303 6.5725 6.96303 6.25592 6.76777 6.06066L5.5 4.79289V3Z" fill="white"/>
                                            </svg> 10 minutes
                                        </div>
                                    </div>
                                </div>
                            </a>
                        </div>
                        </div>
                </div>

                
            </div><!-- container end -->
        </section>
        <section class="bg-white w-full p-4 md:p-12">
            <div class="container mx-auto max-w-screen-xl flex-none"><!-- container start -->   
                <BlogProducts /> 
            </div>
        </section>
</template>