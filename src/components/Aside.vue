<template>
        <aside class="aside">
            <div class="flex-center">
                    <img alt="Vue logo" src="../assets/logo.png">
                        <h1>Aside</h1>
                        <ul>
                            <li v-for="item in list" :key="item">{{item}}</li>
                        </ul>
            </div>
                
            </aside>
</template>
<script>
export default {
    name:'Aside',
    props: [ 'list' ]
}
</script>
