<script setup>
    const logo = {
        fontSize:'28px',
        fontWeight:'bold',
        color:'blue'
    }

    const navContain = {
        home:'Home',
        dropdown:'Dropdown',
        features:'Features',
        pricing:'Pricing',
        about:'About',
        contact:'Contact'
    }
    const signIn = 'sign in'
    const register = 'register'
    const navLink = {
        features:'#features-section',
        pricing:'#pricing-section',
        contact: '#contact-section'
    }

    const promotText = {
        textColor:'text-black',
        fontSize:'text-6xl',
        fontWeight:'font-extrabold'
    }

    const colorlib = {
        color: '#15ECE2',
        backgroundColor: '#E0F9F7',
    }

    const colorlibLink = 'home.com'

    const seeBtn = {
        backgroundColor: '#309490',
        color:'#FFFFFF',
         borderRadius:'10px',
        padding:'5px 14px',
        cursor: 'pointer',
        textTransform: 'capitalize'

    }
    const pricingBtn = {
        border: '0.5px solid #309490',
        color:'#309490',
         borderRadius:'10px',
        padding:'5px 14px',
        cursor: 'pointer',
    }
    const image = {
        src:'https://preview.colorlib.com/theme/launch/images/market-launch-pana.svg',
        alt:'svg image',
        title:'container side image'
    }

    const digitalService = {
        title:'digital services',
        heading:'Selling Digital Services',
        pregraph:'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove right at the coast',
        listOne:'There live the blind texts',
        listTwo:'Far far away behind the word',
        
    }

    const james = {
        name:'James Anderson',
        location:'Facebook, Product Lead',
        spacesJames : '"<em>Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language ocean. A small river named Duden flows by their place and supplies it with the necessary regelialia.</em>"',
        jamesImg :'https://preview.colorlib.com/theme/launch/images/person_1.jpg.webp'

    }
    const videoImg = 'https://preview.colorlib.com/theme/launch/images/dashboard.jpg.webp' 
    const youtubeIcon = {
        position:'absolute',
        top:'50%',
        left:'50%',
        color:'rgb(242, 244, 245)',
        backgroundColor:'red',
        borderRadius:'30px'
    }
    const pricing = {
        heading:'pricing',
        title:'Pricing for everyone.choose your plan now!'
        
    }
    const cardContain = {
            titleOne:'free',
            titleTwo:'standard',
            titleThree:'premium',
            dollar:'$',
            count: 24,
            list:'There live the blind texts',
            buttonText:'get started'

    }
const message = 'false'

if('false' == message){
    cardContain.count = 113;
}

const footerAout = {
    title:'About Launch',
    text:'Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.'

}

const footerProject = {
    title:'Project',
    titleTwo:'Service',
    titleThree:'Location',
    listOne:'La Lega Stadium',
    listTwo:'22 New Homes',
    listThree:'Manage Center',
    listFour:'La Lega Stadium'
}

</script>

<template>
  <section>
    <!--nav section start-->
    <nav class="pt-5 mb-5 w-ful  ">
        <div class=" ">
            <div class="flex justify-between">
                <a href="index.html" :style="logo" class=" float-left pl-5">Launch<span class="text-cyan-600">.</span></a>
                <div class="hidden sm:hidden md:flex lg:flex xl:flex"> 
                    <ul class="flex space-x-5 pt-2 ">
                    <li class="text-xl font-semibold">
                         <a :href="[navLink.features]">{{ navContain.home }}</a>
                    </li>
                    <li class="text-xl font-semibold">
                      <a :href="[navContain.pricing]"> {{ navContain.dropdown }}</a> 
                    </li>
                    <li class="text-xl font-semibold">
                      <a :href="[navContain.contact]">{{ navContain.features }}</a>  
                    </li>
                    <li class="text-xl font-semibold">
                        <a :href="[navContain.contact]">{{ navContain.pricing }}</a>  
                    </li>
                    <li class="text-xl font-semibold">
                        <a :href="[navContain.contact]">{{ navContain.about }}</a>  
                    </li>
                    <li class="text-xl font-semibold">
                        <a :href="[navContain.contact]">{{ navContain.contact }}</a>  
                    </li>
                </ul>
            </div>
            <div class="hidden sm:hidden md:flex lg:flex xl:flex space-x-2 mr-5">
                <button class=" px-4 text-blue-600 text-xl border rounded-full hover:bg-cyan-300 hover:text-blue-700">{{ signIn[0].toUpperCase()+signIn.slice(1) }}</button>
                <button class=" px-4 text-xl border rounded-full capitalize bg-cyan-600 text-white hover:bg-white hover:text-cyan-600">{{ register }}</button>
            </div>
                
            <div class="block sm:block md:hidden lg:hidden xl:hidden">
                <button class="cursor-pointer">
                    <svg width="40px" height="40px" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path fill-rule="evenodd" clip-rule="evenodd" d="M19.5 8.25H4.5V6.75H19.5V8.25Z" fill="#080341"/>
                        <path fill-rule="evenodd" clip-rule="evenodd" d="M19.5 12.75H4.5V11.25H19.5V12.75Z" fill="#080341"/>
                        <path fill-rule="evenodd" clip-rule="evenodd" d="M19.5 17.25H4.5V15.75H19.5V17.25Z" fill="#080341"/>
                    </svg>
                </button>
            </div>
            </div>
        </div>
    </nav>
    <!--nav section end-->
    <!--container section start-->
    <section>
        <div class="py-5 w-full grid grid-cols-1 sm:grid-cols-1 md:grid-cols-2 lg:grid-cols-2 xl:grid-cols-2 pl-5 pt-3">
            <div class="order-2 sm:order-2 md:order-1 lg:order-1">
                <h2 :class=[promotText.textColor,promotText.fontSize,promotText.fontWeight] class="leading-tight">Promote Your <br> Products by <br> Colorlib</h2>
                <div class="w-3/4 pt-2 ">
                    <p class="text-base text-gray-500 leading-7">Another cool free html css template by <a target="_blank" :style="[colorlib]" :href="[colorlibLink]">Colorlib</a> Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove right at the coast</p>
                </div>
                <div class="flex space-x-2 pt-5">
                    <button :style="[seeBtn]">see features</button>
                    <button class="hover:bg-cyan-400 hover:text-white" :style="[pricingBtn]">pricing</button>
                </div>
            </div>
            <div class="order-1 sm:order-1 md:order-2 lg:order-2">
                <img class="w-full" :src='[image.src]' :alt='[image.alt]' :title="[image.title]">
            </div>
        </div>
    </section>
    <!--container section end-->
    <!--digital service section start-->
    <section class="pt-16 pl-5 pb-5">
        <div class="w-full flex flex-col sm:flex-col md:flex-row lg:flex-row">
            <div class="w-full sm:w-full md:w-2/5 lg:w-2/5 pr-5">
                <h3 class="text-xl font-semibold text-cyan-700">{{ digitalService.title.toUpperCase() }}</h3>
                <h3 class="text-lg text-black font-semibold pb-3">{{ digitalService.heading }}</h3>
                <p class="text-base text-gray-500 font-medium pb-2">{{ digitalService.pregraph }}</p>
                <ul class="pb-2">
                    <li class="text-base text-gray-500 font-medium pb-2 flex text-justify">
                        <span><svg style="padding-top: 5px;" fill="#000000" version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" 
                            width="20px" height="20px" viewBox="0 0 335.765 335.765"
                            xml:space="preserve">
                        <g>
                            <g>
                                <polygon points="311.757,41.803 107.573,245.96 23.986,162.364 0,186.393 107.573,293.962 335.765,65.795 		"/>
                            </g>
                        </g>
                        </svg></span>
                    {{ digitalService.listOne }}</li>
                    <li class="text-base text-gray-500 font-medium pb-2 flex text-justify"><span><svg style="padding-top: 5px;" fill="#000000" version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" 
                            width="20px" height="20px" viewBox="0 0 335.765 335.765"
                            xml:space="preserve">
                        <g>
                            <g>
                                <polygon points="311.757,41.803 107.573,245.96 23.986,162.364 0,186.393 107.573,293.962 335.765,65.795 		"/>
                            </g>
                        </g>
                        </svg></span> {{ digitalService.listTwo }}</li>
                </ul>
                <p class="py-3 text-black font-normal text-base" v-html="[james.spacesJames]"></p>
                <div class="flex space-x-3">
                    <img :src="[james.jamesImg]" class="w-12 rounded-full">
                    <div class="block ">
                        <P class="text-black font-normal text-base pb-1">{{ james.name }}</P>
                        <p class="text-gray-400 text-base pb-2">{{ james.location }}</p>
                    </div>
                </div>
            </div>
            <div class="w-full sm:w-full md:w-3/5 lg:w-3/5 py-5">
                <div class="w-3/4 m-auto">
                    <a target="_blank" :href="videoImg" class="relative ">
                        <svg :style="[youtubeIcon]" class="bi bi-play-fill" width="3em" height="3em" viewBox="0 0 16 16" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
                            <path d="M11.596 8.697l-6.363 3.692c-.54.313-1.233-.066-1.233-.697V4.308c0-.63.692-1.01 1.233-.696l6.363 3.692a.802.802 0 0 1 0 1.393z" />
                        </svg>
                        <img :src="videoImg" class="w-full shadow-xl hover:shadow-2xl">
                    </a> 
                </div>
            </div>
        </div>
    </section>
    <!--digital service section end-->

    <!--Pricing section start-->
        <section>
            <div class="pt-10 bg-slate-50 w-full">
                <div class="pt-10 pb-4 w-full text-center">
                    <h2 class="capitalize text-black text-lg font-bold pb-1">{{ pricing.heading }}</h2>
                    <p class="text-gray-500 text-base font-normal">{{ pricing.title }}</p>
                </div>
                <div class="py-10 w-full">
                    <div class="w-9/12 m-auto">
                        <div class="grid grid-cols-1 sm:grid-cols-1 md:grid-cols-3 lg:grid-cols-3 xl:grid-cols-3 gap-3">
                            <div class="bg-white p-6 rounded-lg">
                                <h2 class="capitalize text-xl text-blue-900 font-bold text-center pb-2">{{ cardContain.titleOne }}</h2>
                                <p class="text-center text-blue-700 text-xl font-normal pb-2"><sup>{{ cardContain.dollar }}</sup><span class="font-semibold">0</span></p>
                                <ul class="py-3 ">
                                    <li class="text-base text-gray-500 font-medium pb-2 flex text-justify">
                                        <span >
                                        <svg style="padding-top: 5px;" fill="#000000" version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" 
                                             width="20px" height="20px" viewBox="0 0 335.765 335.765"
                                             xml:space="preserve">
                                            <g>
                                                <g>
                                                    <polygon points="311.757,41.803 107.573,245.96 23.986,162.364 0,186.393 107.573,293.962 335.765,65.795 		"/>
                                                </g>
                                            </g>
                                        </svg>
                                    </span>
                                   <span>{{ cardContain.list }}</span> </li>
                                   <li class="text-base text-gray-500 font-medium pb-2 flex text-justify">
                                        <span >
                                        <svg style="padding-top: 5px;" fill="#000000" version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" 
                                             width="20px" height="20px" viewBox="0 0 335.765 335.765"
                                             xml:space="preserve">
                                            <g>
                                                <g>
                                                    <polygon points="311.757,41.803 107.573,245.96 23.986,162.364 0,186.393 107.573,293.962 335.765,65.795 		"/>
                                                </g>
                                            </g>
                                        </svg>
                                    </span>
                                   <span>{{ cardContain.list }}</span> </li>
                                   <li class="text-base text-gray-500 font-medium pb-2 flex text-justify">
                                        <span >
                                        <svg style="padding-top: 5px;" fill="#000000" version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" 
                                             width="20px" height="20px" viewBox="0 0 335.765 335.765"
                                             xml:space="preserve">
                                            <g>
                                                <g>
                                                    <polygon points="311.757,41.803 107.573,245.96 23.986,162.364 0,186.393 107.573,293.962 335.765,65.795 		"/>
                                                </g>
                                            </g>
                                        </svg>
                                    </span>
                                   <span>{{ cardContain.list }}</span> </li>
                                   <li class="text-base text-gray-500 font-medium pb-2 flex text-justify">
                                        <span >
                                        <svg style="padding-top: 5px;" fill="#000000" version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" 
                                             width="20px" height="20px" viewBox="0 0 335.765 335.765"
                                             xml:space="preserve">
                                            <g>
                                                <g>
                                                    <polygon points="311.757,41.803 107.573,245.96 23.986,162.364 0,186.393 107.573,293.962 335.765,65.795 		"/>
                                                </g>
                                            </g>
                                        </svg>
                                    </span>
                                   <span>{{ cardContain.list }}</span> </li>
                                </ul>
                                <div class="py-4 w-full text-center">
                                    <button class="py-1 px-4 border-cyan-400 border rounded-full cursor-pointer capitalize text-lg text-cyan-400 font-normal">{{ cardContain.buttonText }}</button>
                                </div>
                            </div>
                            <div class="bg-white p-6 rounded-lg">
                                <h2 class="capitalize text-xl text-blue-900 font-bold text-center pb-2">{{ cardContain.titleTwo }}</h2>
                                <p class="text-center text-blue-700 text-xl font-normal pb-2"><sup>{{ cardContain.dollar }}</sup><span class="font-semibold">{{ cardContain.count / 5 }}</span></p>
                                <ul class="py-3 ">
                                    <li class="text-base text-gray-500 font-medium pb-2 flex text-justify">
                                        <span >
                                        <svg style="padding-top: 5px;" fill="#000000" version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" 
                                             width="20px" height="20px" viewBox="0 0 335.765 335.765"
                                             xml:space="preserve">
                                            <g>
                                                <g>
                                                    <polygon points="311.757,41.803 107.573,245.96 23.986,162.364 0,186.393 107.573,293.962 335.765,65.795 		"/>
                                                </g>
                                            </g>
                                        </svg>
                                    </span>
                                   <span>{{ cardContain.list }}</span> </li>
                                   <li class="text-base text-gray-500 font-medium pb-2 flex text-justify">
                                        <span >
                                        <svg style="padding-top: 5px;" fill="#000000" version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" 
                                             width="20px" height="20px" viewBox="0 0 335.765 335.765"
                                             xml:space="preserve">
                                            <g>
                                                <g>
                                                    <polygon points="311.757,41.803 107.573,245.96 23.986,162.364 0,186.393 107.573,293.962 335.765,65.795 		"/>
                                                </g>
                                            </g>
                                        </svg>
                                    </span>
                                   <span>{{ cardContain.list }}</span> </li>
                                   <li class="text-base text-gray-500 font-medium pb-2 flex text-justify">
                                        <span >
                                        <svg style="padding-top: 5px;" fill="#000000" version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" 
                                             width="20px" height="20px" viewBox="0 0 335.765 335.765"
                                             xml:space="preserve">
                                            <g>
                                                <g>
                                                    <polygon points="311.757,41.803 107.573,245.96 23.986,162.364 0,186.393 107.573,293.962 335.765,65.795 		"/>
                                                </g>
                                            </g>
                                        </svg>
                                    </span>
                                   <span>{{ cardContain.list }}</span> </li>
                                   <li class="text-base text-gray-500 font-medium pb-2 flex text-justify">
                                        <span >
                                        <svg style="padding-top: 5px;" fill="#000000" version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" 
                                             width="20px" height="20px" viewBox="0 0 335.765 335.765"
                                             xml:space="preserve">
                                            <g>
                                                <g>
                                                    <polygon points="311.757,41.803 107.573,245.96 23.986,162.364 0,186.393 107.573,293.962 335.765,65.795 		"/>
                                                </g>
                                            </g>
                                        </svg>
                                    </span>
                                   <span>{{ cardContain.list }}</span> </li>
                                </ul>
                                <div class="py-4 w-full text-center">
                                    <button class="py-1 px-4 border-cyan-500 border bg-cyan-500 rounded-full cursor-pointer capitalize text-lg text-white font-normal hover:bg-white hover:text-cyan-500">{{ cardContain.buttonText }}</button>
                                </div>
                            </div>
                            <div class="bg-white p-6 rounded-lg">
                                <h2 class="capitalize text-xl text-blue-900 font-bold text-center pb-2">{{ cardContain.titleThree }}</h2>
                                <p class="text-center text-blue-700 text-xl font-normal pb-2"><sup>{{ cardContain.dollar }}</sup><span class="font-semibold">{{ cardContain.count / 2 }}</span></p>
                                <ul class="py-3 ">
                                    <li class="text-base text-gray-500 font-medium pb-2 flex text-justify">
                                        <span >
                                        <svg style="padding-top: 5px;" fill="#000000" version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" 
                                             width="20px" height="20px" viewBox="0 0 335.765 335.765"
                                             xml:space="preserve">
                                            <g>
                                                <g>
                                                    <polygon points="311.757,41.803 107.573,245.96 23.986,162.364 0,186.393 107.573,293.962 335.765,65.795 		"/>
                                                </g>
                                            </g>
                                        </svg>
                                    </span>
                                   <span>{{ cardContain.list }}</span> </li>
                                   <li class="text-base text-gray-500 font-medium pb-2 flex text-justify">
                                        <span >
                                        <svg style="padding-top: 5px;" fill="#000000" version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" 
                                             width="20px" height="20px" viewBox="0 0 335.765 335.765"
                                             xml:space="preserve">
                                            <g>
                                                <g>
                                                    <polygon points="311.757,41.803 107.573,245.96 23.986,162.364 0,186.393 107.573,293.962 335.765,65.795 		"/>
                                                </g>
                                            </g>
                                        </svg>
                                    </span>
                                   <span>{{ cardContain.list }}</span> </li>
                                   <li class="text-base text-gray-500 font-medium pb-2 flex text-justify">
                                        <span >
                                        <svg style="padding-top: 5px;" fill="#000000" version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" 
                                             width="20px" height="20px" viewBox="0 0 335.765 335.765"
                                             xml:space="preserve">
                                            <g>
                                                <g>
                                                    <polygon points="311.757,41.803 107.573,245.96 23.986,162.364 0,186.393 107.573,293.962 335.765,65.795 		"/>
                                                </g>
                                            </g>
                                        </svg>
                                    </span>
                                   <span>{{ cardContain.list }}</span> </li>
                                   <li class="text-base text-gray-500 font-medium pb-2 flex text-justify">
                                        <span >
                                        <svg style="padding-top: 5px;" fill="#000000" version="1.1" id="Capa_1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" 
                                             width="20px" height="20px" viewBox="0 0 335.765 335.765"
                                             xml:space="preserve">
                                            <g>
                                                <g>
                                                    <polygon points="311.757,41.803 107.573,245.96 23.986,162.364 0,186.393 107.573,293.962 335.765,65.795 		"/>
                                                </g>
                                            </g>
                                        </svg>
                                    </span>
                                   <span>{{ cardContain.list }}</span> </li>
                                </ul>
                                <div class="py-4 w-full text-center">
                                    <button class="py-1 px-4 border-cyan-400 border rounded-full cursor-pointer capitalize text-lg text-cyan-400 font-normal">{{ cardContain.buttonText }}</button>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    <!--Pricing section end-->

    <!--footer section start-->
        <section>
            <div class="pt-16 bg-gray-100 pb-10">
                <div class="px-5 flex flex-col sm:flex-col md:flex-col lg:flex-row xl:flex-row w-full gap-3">
                    <div class="w-full sm:w-full md:w-full lg:w-2/5">
                        <h2 class="text-lg font-bold text-gray-500">{{ footerAout.title }}</h2>
                        <p class="pt-8 text-gray-500 text-base">{{ footerAout.text }}</p>
                    </div>
                    <div class="w-full sm:w-full md:w-full lg:w-3/5">
                       <div class="grid grid-cols-1 sm:grid-cols-1 md:grid-cols-3 lg:grid-cols-3 gap-3">
                            <div class="">
                                <h2 class="text-lg font-bold text-gray-500 pb-5">{{ footerProject.title }}</h2>
                                <p class="text-base text-gray-500 font-medium pb-2">{{ footerProject.listOne }}</p>
                                <p class="text-base text-gray-500 font-medium pb-2">{{ footerProject.listTwo }}</p>
                                <p class="text-base text-gray-500 font-medium pb-2">{{ footerProject.listThree }}</p>
                                <p class="text-base text-gray-500 font-medium pb-2">{{ footerProject.listFour }}</p>
                            </div>
                            <div class="">
                                <h2 class="text-lg font-bold text-gray-500 pb-5">{{ footerProject.titleTwo }}</h2>
                                <p class="text-base text-gray-500 font-medium pb-2">{{ footerProject.listOne }}</p>
                                <p class="text-base text-gray-500 font-medium pb-2">{{ footerProject.listTwo }}</p>
                                <p class="text-base text-gray-500 font-medium pb-2">{{ footerProject.listThree }}</p>
                                <p class="text-base text-gray-500 font-medium pb-2">{{ footerProject.listFour }}</p>
                            </div>
                            <div class=" ">
                                <h2 class="text-lg font-bold text-gray-500 pb-5">{{ footerProject.titleThree }}</h2>
                                <p class="text-base text-gray-500 font-medium pb-2">{{ footerProject.listOne }}</p>
                                <p class="text-base text-gray-500 font-medium pb-2">{{ footerProject.listTwo }}</p>
                                <p class="text-base text-gray-500 font-medium pb-2">{{ footerProject.listThree }}</p>
                                <p class="text-base text-gray-500 font-medium pb-2">{{ footerProject.listFour }}</p>
                            </div>
                       </div>
                    </div>
                </div>
            </div>
        </section>
    <!--footer section end-->
  </section>
</template>

<style scoped>

</style>
