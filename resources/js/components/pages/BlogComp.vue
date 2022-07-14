<template>
    <div>
        <h1>Tutti i Post</h1>
        <ul>

            <li v-for="post in posts" :key="post.id">


                <h1>{{post.title}}</h1>
                <p>{{post.contenet}}</p>
            </li>

        </ul>
    </div>
</template>

<script>
import axios from 'axios'

export default {
name:'BlogComp',

    data() {
        return {
            posts:null
        }
    },
    mounted() {

        this.getApi()


    },

    methods: {
        getApi(){
            axios.get('/api/posts')
            .then(res =>{

                this.posts=res.data;
            })
        }
    },
}
</script>

<style>

</style>
