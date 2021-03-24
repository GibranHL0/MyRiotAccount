<template>
    <div class="p-8" >
        <div id="searcher" class="bg-gray-600 flex items-center rounded-t-2xl rounded-b-2xl
        bg-opacity-95 h-14">
            <input v-model="summoner" class="rounded-l-fully w-full py-4 px-6 bg-gray-700 leading-tight
            focus:outline-none text-white rounded-t-2xl rounded-b-2xl bg-opacity-0" 
            type="text" placeholder="Summoner Name.." v-on:keyup.enter="searchSummoner()">
            <div class="pl-1">
                <select v-model="selected_region" name="region-options" id="region-options"
                class="bg-gray-700 hover:bg-gray-900 rounded-t-xl rounded-b-xl
                 text-white p-2 w-15 h-14">
                    <option v-for="region in regions" v-bind:key="region" :value="region">
                        {{region[0]}}
                    </option>
                </select>
            </div>
        </div>
    </div>
</template>

<script>
export default{
    setup(){
        const selected_region = ["LAN","LA1"];
        const summoner = "";
        return {selected_region, summoner}
    },
    data(){
        return {
            regions: [["LAN","LA1"],["LAS","LA2"],["BR","BR1"],["EUE","EUN1"],["EUW","EUW1"],
                     ["JN","JP1"],["KR","KR"],["NA","NA1"],["OCE","OC1"],["TUR","TR1"],["RU","RU"]]
        }
    },
    methods: {
        searchSummoner(){
            console.log(this.summoner)
            console.log(this.selected_region[1])
        }
    }
}
</script>
