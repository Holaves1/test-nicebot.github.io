<template>
    <div class="header-page">
        <Navbar></Navbar>
    </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue'

export default{
    components:{
        Navbar
    }
}

</script>

<style lang="scss" scoped>
    .header-page{
        background-image: url(@/assets/header-bg-V1.jpg);
        background-repeat: no-repeat;
        background-position: right ;
        background-size: cover;
        min-height: 120vh;
        width: 100%;
    }
</style>