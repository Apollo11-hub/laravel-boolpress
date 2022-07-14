<template>
    <header>
        <nav>
            <ul>
                <li>
                    <router-link :to="{name:'home'}">Home</router-link>
                </li>
                <li>
                    <router-link :to="{name:'blog'}">Blog</router-link>
                </li>
                <li>
                    <router-link :to="{name:'about'}" >Chi Siamo</router-link>
                </li>
                <li>
                    <router-link :to="{name:'contacts'}" >Contatti</router-link>
                </li>

            </ul>
        </nav>
    </header>
</template>

<script>
export default {
name:'HeaderComp',

}
</script>

<style lang="scss" scoperd>
    header{
        background-color: rgb(128, 130, 240);
        ul{
            display:flex;
            justify-content: center;
            padding: 10px 0 ;
            li{
                margin: 0 10px;
                list-style:none;
                a{
                    text-decoration: none;
                    &.active,
                    &:hover{
                        color:red;
                    }
                }
            }
        }
    }

</style>
