<script>
import Chart from 'chart.js/auto';
import { getRelativePosition } from 'chart.js/helpers';
export default {
    
    data() {
        return {
            config1: {
        type: 'line',
        data: {
          labels: [],
          datasets: [{
            label: 'Totaal Meldingen',
            data: [],
            lineTension: 0,
            backgroundColor: [
              'rgba(43,88,130,0.4)',
            ],
            pointRadius: 1,
            pointHoverRadius: 1,
            fill: true,
            redraw: true,
            borderColor: [
              'rgba(31,65,96)',

            ],
            borderWidth: 3
          }]
        },
        options: {    
            onClick: (e) => {
                    const canvasPosition = getRelativePosition(e, chart);

                    // Substitute the appropriate scale IDs
                    const dataX = chart.scales.x.getValueForPixel(canvasPosition.x);
                    const dataY = chart.scales.y.getValueForPixel(canvasPosition.y);
                    },
          scales: {
            y: {
              display: false
            },
            ticks: {
              display: false
            }
          },

          elements: {
            point: {
              radius: 0
            }
          },
          plugins: {
            legend: {
              display: false
            },
            tooltip: {
              position: 'nearest',
              padding: 10,
              cornerRadius: 10,
              backgroundColor: 'rgba(43,88,133)',
              callbacks: {
                label: function (context) {
                  return context.parsed.y;
                },
                title: () => null
              },

              yAlign: 'bottom',
              displayColors: false,

            }
          }
        }
      },
      myChart1: null,
        }
    },
    mounted() {
        this.ChartRender()
    },
    methods: {
        ChartRender() {
      if (this.myChart1 != null) {
        this.myChart1.destroy();
      }
      this.myChart1 = new Chart(
        document.getElementById('myChart1'),
        this.config1
      );

    },
    }
}
</script>
<script setup>
import { onMounted } from 'vue'
    import { Modal } from 'flowbite'

    // initialize components based on data attribute selectors
    onMounted(() => {
    const $buttonElement = document.querySelector('.modal-btn');
    const $modalElement = document.querySelector('#large-modal');
    const $closeButton = document.querySelector('#closeButton');

    const modalOptions = {
        backdropClasses: 'bg-gray-900 bg-opacity-50 dark:bg-opacity-80 fixed inset-0 z-40'
    }

    if ($modalElement) {
        const modal = new Modal($modalElement, modalOptions);
        $buttonElement.addEventListener('click', () => modal.toggle());
        $closeButton.addEventListener('click', () => modal.hide());
        
        // programmatically show
        // modal.show();
    }
})
</script>
<template>
        <div id="large-modal" tabindex="-1" aria-hidden="true" class="fixed top-0 left-0 right-0 z-50 hidden w-full  p-8 overflow-x-hidden overflow-y-auto md:inset-0 h-modal md:h-full">
        <div class="relative w-full h-full md:w-[805px] md:h-auto">
            <!-- Modal content -->
            <div class="relative bg-white rounded-lg shadow dark:bg-gray-700">
                <!-- Modal header -->
                <div class="flex items-start justify-between">
                    
                    <button id="closeButton" type="button" class="text-gray-400 bg-transparent hover:bg-gray-200 hover:text-gray-900 rounded-lg text-sm p-1.5 ml-auto inline-flex items-center dark:hover:bg-gray-600 dark:hover:text-white">
                        <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><path fill-rule="evenodd" d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z" clip-rule="evenodd"></path></svg>  
                    </button>
                </div>
                <!-- Modal body -->
                <div class="p-6 space-y-6">
                    <div class="modal-product-info flex-col flex md:flex-row align-middle justify-between">
                        <div class="img-box flex justify-center items-center relative h-[165px] w-full md:w-[273px] bg-[#F5F8FF]">
                            <div class="product-img p-8">
                                <img class="object-cover w-auto rounded-t-lg h-auto mx-auto" src="@/assets/img/offers/keyboard.png"
                                    alt="image">
                            </div>
                            <div class="brand-logo">
                                <img src="@/assets/img/providers/bol.com.png" alt="icon">
                            </div>
                        </div>
                        <div class="product-details-s w-full pl-5">
                            <h3 class="text-[#2B313B] font-bold text-xl mb-3">K380 MULTI-DEVICE KEYBOARD FOR MAC</h3>
                            <div class="rating-area flex align-middle justify-start mb-5">
                                <svg width="18" height="17" viewBox="0 0 18 17" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8.13024 0.533005C8.51342 -0.142371 9.48658 -0.142372 9.86976 0.533003L11.9616 4.22001C12.1041 4.47108 12.3481 4.64834 12.6308 4.70623L16.7838 5.55636C17.5445 5.71208 17.8453 6.63762 17.3214 7.21075L14.4612 10.3396C14.2665 10.5526 14.1733 10.8394 14.2056 11.1263L14.6804 15.3387C14.7674 16.1103 13.9801 16.6823 13.2731 16.3612L9.4136 14.6079C9.15079 14.4885 8.84921 14.4885 8.5864 14.6079L4.72688 16.3612C4.0199 16.6823 3.23259 16.1103 3.31957 15.3387L3.79439 11.1263C3.82672 10.8395 3.73353 10.5526 3.53877 10.3396L0.678637 7.21075C0.154726 6.63762 0.45545 5.71208 1.21618 5.55636L5.36916 4.70623C5.65195 4.64834 5.89593 4.47108 6.03838 4.22002L8.13024 0.533005Z" fill="#EFBC21"/>
</svg>
<svg width="18" height="17" viewBox="0 0 18 17" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8.13024 0.533005C8.51342 -0.142371 9.48658 -0.142372 9.86976 0.533003L11.9616 4.22001C12.1041 4.47108 12.3481 4.64834 12.6308 4.70623L16.7838 5.55636C17.5445 5.71208 17.8453 6.63762 17.3214 7.21075L14.4612 10.3396C14.2665 10.5526 14.1733 10.8394 14.2056 11.1263L14.6804 15.3387C14.7674 16.1103 13.9801 16.6823 13.2731 16.3612L9.4136 14.6079C9.15079 14.4885 8.84921 14.4885 8.5864 14.6079L4.72688 16.3612C4.0199 16.6823 3.23259 16.1103 3.31957 15.3387L3.79439 11.1263C3.82672 10.8395 3.73353 10.5526 3.53877 10.3396L0.678637 7.21075C0.154726 6.63762 0.45545 5.71208 1.21618 5.55636L5.36916 4.70623C5.65195 4.64834 5.89593 4.47108 6.03838 4.22002L8.13024 0.533005Z" fill="#EFBC21"/>
</svg>
<svg width="18" height="17" viewBox="0 0 18 17" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8.13024 0.533005C8.51342 -0.142371 9.48658 -0.142372 9.86976 0.533003L11.9616 4.22001C12.1041 4.47108 12.3481 4.64834 12.6308 4.70623L16.7838 5.55636C17.5445 5.71208 17.8453 6.63762 17.3214 7.21075L14.4612 10.3396C14.2665 10.5526 14.1733 10.8394 14.2056 11.1263L14.6804 15.3387C14.7674 16.1103 13.9801 16.6823 13.2731 16.3612L9.4136 14.6079C9.15079 14.4885 8.84921 14.4885 8.5864 14.6079L4.72688 16.3612C4.0199 16.6823 3.23259 16.1103 3.31957 15.3387L3.79439 11.1263C3.82672 10.8395 3.73353 10.5526 3.53877 10.3396L0.678637 7.21075C0.154726 6.63762 0.45545 5.71208 1.21618 5.55636L5.36916 4.70623C5.65195 4.64834 5.89593 4.47108 6.03838 4.22002L8.13024 0.533005Z" fill="#EFBC21"/>
</svg>
<svg width="18" height="17" viewBox="0 0 18 17" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8.13024 0.533005C8.51342 -0.142371 9.48658 -0.142372 9.86976 0.533003L11.9616 4.22001C12.1041 4.47108 12.3481 4.64834 12.6308 4.70623L16.7838 5.55636C17.5445 5.71208 17.8453 6.63762 17.3214 7.21075L14.4612 10.3396C14.2665 10.5526 14.1733 10.8394 14.2056 11.1263L14.6804 15.3387C14.7674 16.1103 13.9801 16.6823 13.2731 16.3612L9.4136 14.6079C9.15079 14.4885 8.84921 14.4885 8.5864 14.6079L4.72688 16.3612C4.0199 16.6823 3.23259 16.1103 3.31957 15.3387L3.79439 11.1263C3.82672 10.8395 3.73353 10.5526 3.53877 10.3396L0.678637 7.21075C0.154726 6.63762 0.45545 5.71208 1.21618 5.55636L5.36916 4.70623C5.65195 4.64834 5.89593 4.47108 6.03838 4.22002L8.13024 0.533005Z" fill="#EFBC21"/>
</svg>
<svg width="18" height="17" viewBox="0 0 18 17" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8.13024 0.533005C8.51342 -0.142371 9.48658 -0.142372 9.86976 0.533003L11.9616 4.22001C12.1041 4.47108 12.3481 4.64834 12.6308 4.70623L16.7838 5.55636C17.5445 5.71208 17.8453 6.63762 17.3214 7.21075L14.4612 10.3396C14.2665 10.5526 14.1733 10.8394 14.2056 11.1263L14.6804 15.3387C14.7674 16.1103 13.9801 16.6823 13.2731 16.3612L9.4136 14.6079C9.15079 14.4885 8.84921 14.4885 8.5864 14.6079L4.72688 16.3612C4.0199 16.6823 3.23259 16.1103 3.31957 15.3387L3.79439 11.1263C3.82672 10.8395 3.73353 10.5526 3.53877 10.3396L0.678637 7.21075C0.154726 6.63762 0.45545 5.71208 1.21618 5.55636L5.36916 4.70623C5.65195 4.64834 5.89593 4.47108 6.03838 4.22002L8.13024 0.533005Z" fill="#A4BCE6"/>
</svg>
<span class="review-status text-xs text-[#2B313B] font-bold ml-2">8.5</span><span class="total-review text-xs text[#6C7A93] font-normal ml-2">(10089 Reviews)</span>
                            </div>
                            <button type="button" class="add-notification bg-[#FFF6F3] flex align-middle justify-between w-full p-3">
                                <div class="flex items-center">
                                    <span class="notification-icon mr-2">
                                        <svg width="14" height="10" viewBox="0 0 14 10" fill="none" xmlns="http://www.w3.org/2000/svg">
                                            <path d="M0.602276 1.70704L6.99957 4.90568L13.3969 1.707C13.3487 0.866717 12.652 0.200195 11.7996 0.200195H2.19961C1.34722 0.200195 0.650517 0.866739 0.602276 1.70704Z" fill="#FC7428"/>
                                            <path d="M13.3996 3.49452L6.99957 6.69454L0.599609 3.49456V8.2002C0.599609 9.08385 1.31595 9.8002 2.19961 9.8002H11.7996C12.6833 9.8002 13.3996 9.08385 13.3996 8.2002V3.49452Z" fill="#FC7428"/>
                                            </svg>
                                    </span>
                                    <span class="text=[#FC7428] text-sm font-normal">Set Notification for this Product</span>
                                </div>
                                <div>
                                    <svg width="15" height="15" viewBox="0 0 15 15" fill="none" xmlns="http://www.w3.org/2000/svg">
                                        <path d="M5.33789 1.52918C5.22354 1.10241 4.78487 0.84914 4.35809 0.963493C3.93132 1.07785 3.67805 1.51652 3.79241 1.94329L3.99946 2.71603C4.11382 3.1428 4.55249 3.39607 4.97926 3.28172C5.40603 3.16736 5.6593 2.72869 5.54494 2.30192L5.33789 1.52918Z" fill="#112954"/>
                                        <path d="M1.94378 3.79192C1.517 3.67757 1.07833 3.93083 0.963981 4.35761C0.849628 4.78438 1.10289 5.22305 1.52967 5.3374L2.30241 5.54446C2.72918 5.65881 3.16785 5.40554 3.2822 4.97877C3.39656 4.552 3.14329 4.11333 2.71652 3.99898L1.94378 3.79192Z" fill="#112954"/>
                                        <path d="M8.99454 3.3372C9.30696 3.02478 9.30696 2.51824 8.99454 2.20582C8.68212 1.89341 8.17559 1.8934 7.86317 2.20582L7.29748 2.77151C6.98506 3.08393 6.98506 3.59046 7.29748 3.90288C7.6099 4.2153 8.11643 4.2153 8.42885 3.90288L8.99454 3.3372Z" fill="#112954"/>
                                        <path d="M3.33768 8.99405L3.90337 8.42836C4.21579 8.11595 4.21579 7.60941 3.90337 7.29699C3.59095 6.98457 3.08442 6.98457 2.772 7.29699L2.20631 7.86268C1.89389 8.1751 1.89389 8.68163 2.20631 8.99405C2.51873 9.30647 3.02526 9.30647 3.33768 8.99405Z" fill="#112954"/>
                                        <path d="M5.89762 4.85721C5.60049 4.73836 5.26111 4.80802 5.03482 5.03431C4.80853 5.2606 4.73888 5.59997 4.85773 5.89711L8.05773 13.8971C8.17473 14.1896 8.4525 14.3862 8.76726 14.3993C9.08203 14.4124 9.37516 14.2395 9.51605 13.9578L10.6197 11.7505L13.0348 14.1657C13.3472 14.4781 13.8538 14.4781 14.1662 14.1657C14.4786 13.8533 14.4786 13.3467 14.1662 13.0343L11.751 10.6192L13.9583 9.51554C14.2401 9.37465 14.4129 9.08151 14.3998 8.76675C14.3867 8.45199 14.1901 8.17421 13.8976 8.05721L5.89762 4.85721Z" fill="#112954"/>
                                    </svg>
                                </div>
                            </button>
                        </div>
                        <div class="chart-wrapper">
                            <div ref="aanbiending24" class="">
                      <canvas id="myChart1" width="400" height="400"></canvas>
                    </div>
                        </div>
                    </div>
                    <p class="text-base leading-relaxed text-gray-500 dark:text-gray-400">
                        With less than a month to go before the European Union enacts new consumer privacy laws for its citizens, companies around the world are updating their terms of service agreements to comply.
                    </p>
                    <p class="text-base leading-relaxed text-gray-500 dark:text-gray-400">
                        The European Union’s General Data Protection Regulation (G.D.P.R.) goes into effect on May 25 and is meant to ensure a common set of data rights in the European Union. It requires organizations to notify users as soon as possible of high-risk data breaches that could personally affect them.
                    </p>
                </div>
                <!-- Modal footer -->
                <div class="flex items-center p-6 space-x-2 border-t border-gray-200 rounded-b dark:border-gray-600">
                    <button type="button" class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">I accept</button>
                    <button type="button" class="text-gray-500 bg-white hover:bg-gray-100 focus:ring-4 focus:outline-none focus:ring-blue-300 rounded-lg border border-gray-200 text-sm font-medium px-5 py-2.5 hover:text-gray-900 focus:z-10 dark:bg-gray-700 dark:text-gray-300 dark:border-gray-500 dark:hover:text-white dark:hover:bg-gray-600">Decline</button>
                </div>
            </div>
        </div>
    </div>
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

                <!-- product table end -->

            </div><!-- container end -->
        </section>
</template>