<template>
    <div>
            <HeaderComp></HeaderComp>
            <router-view></router-view>
    </div>
</template>

<script>
import axios from 'axios'
import HeaderComp from './components/partials/HeaderComp.vue'

export default {
    name:'App',
    components:{HeaderComp},

    // data() {
    //     return {
    //         posts:null
    //     }
    // },
    // mounted() {

    //     this.getApi()


    // },

    // methods: {
    //     getApi(){
    //         axios.get('/api/posts')
    //         .then(res =>{
    //             this.posts=res.data;
    //         })
    // //     }
    // },
}
</script>

<style>

</style>
