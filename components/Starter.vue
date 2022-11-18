<template>
  <div class="relative flex flex-col items-top justify-center min-h-screen bg-gank-gray">
    <header class="w-full bg-gank-gray fixed top-0 left-0 z-10">
        <div class="w-full flex justify-between items-center 2xl:mx-auto 2xl:w-[1500px] py-5 h-[90px]">
            <div class="block">
                <nuxt-logo/>
            </div>
            <div class="right flex items-center pr-10">
                <button class="mx-2">
                    <div class="w-12 h-12 p-1">
                        <svg viewBox="0 0 24 24" focusable="false" class="stroke-current fill-white style-scope text-white" style="pointer-events: none; display: block; width: 100%; height: 100%;">
                            <g class="stroke-current fill-current style-scope">
                            <path d="M10,20h4c0,1.1-0.9,2-2,2S10,21.1,10,20z M20,17.35V19H4v-1.65l2-1.88v-5.15c0-2.92,1.56-5.22,4-5.98V3.96 c0-1.42,1.49-2.5,2.99-1.76C13.64,2.52,14,3.23,14,3.96l0,0.39c2.44,0.75,4,3.06,4,5.98v5.15L20,17.35z M19,17.77l-2-1.88v-5.47 c0-2.47-1.19-4.36-3.13-5.1c-1.26-0.53-2.64-0.5-3.84,0.03C8.15,6.11,7,7.99,7,10.42v5.47l-2,1.88V18h14V17.77z" class="stroke-current fill-current style-scope yt-icon"></path>
                            </g>
                        </svg>
                    </div>
                </button>
            </div>
        </div>
    </header>
    <div class="dark w-full 2xl:w-[1500px] 2xl:mx-auto relative grid grid-cols-10 pt-[90px]">
        <div class=" col-span-2 sm:col-span-4 lg:col-span-2">
            <side-menu />
        </div>
        <div class="col-span-8 sm:col-span-6 lg:col-span-4 h-full flex flex-col ">
            <list/>
        </div>
    </div>
    </div>
</template>

<script>
import NuxtLogo from './NuxtLogo.vue'
export default {
  name: 'Starter'
}
</script>
