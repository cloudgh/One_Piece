<template>
    <div class="app">
        <router-view></router-view>
    </div>
</template>

<script>
    export default {
         name: 'App'}
</script>
<style lang="scss">

#app {
    background: #C0C0C0;
}

* {  
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    // background-image: url('@/assets/images1.jpg'); 
    background-size: cover; 
    background-repeat: no-repeat;
    background-attachment: fixed; 
}


</style>