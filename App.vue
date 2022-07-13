<template>
        <div class="app">
            <router-view></router-view>
        </div>
</template>

<script>


export default{

}

</script>

<style lang="scss" >
    *{
        box-sizing: border-box;
        padding: 0;
        margin: 0;
    }
    ._container{
        max-width: 1110px;
        overflow: hidden;
        margin: 0 auto;
        width: 100%;
    }
    :active, :hover, :focus {
        outline: 0;
        outline-offset: 0;
    }
</style>