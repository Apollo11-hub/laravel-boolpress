<template>
    <div>
            <HeaderComp></HeaderComp>
            <router-view></router-view>
    </div>
</template>

<script>

import HeaderComp from './components/partials/HeaderComp.vue'

export default {
    name:'App',
    components:{HeaderComp},


}
</script>

<style>

</style>
