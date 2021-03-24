<template>
    <div id="welcome" class="space-y-6 w-full">
        <div id="header" :style="{'background-image': 'url(' + require('./assets/home/home.jpg') + ')', 
        'background-repeat':'no-repeat', 'background-size': 'cover'}"
        class="h-96">
            <h2 class="text-5xl text-white text-center p-10 font-bold">
                Welcome to My Riot Account
            </h2>
            <div class="flex justify-center">
                <Searcher class="w-1/3"/>
            </div>
            <div class="flex justify-center pt-8">
                <button class=" bg-black text-white rounded-2xl text-2xl pr-4 pl-4 h-11
                 border-white border-2 hover:bg-red-800">
                    WIN PREDICTION
                </button>
            </div>
        </div>
        <div id="products" class="text-white pt-10">
            <h2 class="text-center text-5xl">
                What is this project?
            </h2>
            <div class="flex space x-3 pt-16">
                <div class="inline-block w-1/3">
                    <div class="flex justify-center">
                        <div>
                            <h2 class="text-center text-2xl">
                                Stats
                            </h2>
                            <img class="w-32" src="./assets/home/stats.png"/>
                        </div>
                    </div>
                </div>
                <div class="inline-block w-1/3">
                    <div class="flex justify-center">
                        <div>
                            <h2 class="text-center text-2xl">
                                Rank Info
                            </h2>
                            <img class="w-32" src="./assets/home/chevron.png"/>
                        </div>
                    </div>
                </div>
                <div class="inline-block w-1/3">
                    <div class="flex justify-center">
                        <div>
                            <h2 class="text-center text-2xl">
                                Win Prediction
                            </h2>
                            <img class="w-32" src="./assets/home/analytics.png"/>
                        </div>
                    </div>
                </div>
            </div>
            <div class="pt-20">
                <h2 class="text-center text-4xl">
                    All the information from your rank games!
                </h2>
            </div>
        </div>
        <div id="league-logo" class="flex justify-center pt-16">
            <img class="w-1/5" src="./assets/home/league_logo.png">
        </div>
        <div id="tech" class="text-white pt-16">
            <h2 class="text-center text-5xl mt-4">
                Powered by
            </h2>
            <div class="flex space-x-3 mt-10">
                <div class="inline-block w-1/3">
                    <div class="flex justify-center">
                        <div>
                            <img class="w-44 pt-6" src="./assets/home/tailwind-css-logo.svg"/>
                            <h2 class="text-center text-2xl pt-4">
                                Tailwind
                            </h2>
                        </div>
                    </div>
                </div>
                <div class="inline-block w-1/3">
                    <div class="flex justify-center">
                        <div>
                            <img class="w-44" src="./assets/home/vueLogo.png"/>
                            <h2 class="text-center text-2xl">
                                VueJS
                            </h2>
                        </div>
                    </div>
                </div>
                <div class="inline-block w-1/3">
                    <div class="flex justify-center">
                        <div>
                            <img class="w-32 pt-6" src="./assets/home/flask_logo.png"/>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div id="author" class="pt-20 pl-24 flex space-x-2">
            <div id="created" class="flex-1">
                <div class="relative h-full w-full">
                    <div class="absolute inset-y-1/3 right-0">
                        <h2 class="text-white text-5xl pr-24"> 
                            Created By 
                        </h2>
                    </div>
                </div>
            </div>
            <div class="flex-1">
                <div id="me-picture" class="bg-white rounded-3xl p-4 w-1/5">
                    <div class="block">
                        <div class="flex justify-center">
                            <img class="w-40 rounded" src="./assets/home/me.jpg">
                        </div>
                    </div>
                    <div class="block text-center pt-4">
                        <h2 class=" text-3xl">
                            Gibran Herrera
                        </h2>
                    </div>
                </div>
            </div>
        </div>
        <div id="footer" class="flex pt-16">
            <Footer class="w-screen"/>
        </div>
    </div>
</template>

<script>
import Searcher from './components/Searcher.vue';
import Footer from './components/Footer.vue';

export default{
    setup() {
    },
    methods: {

    },
    components:{
        Searcher,
        Footer
    }
}
</script>