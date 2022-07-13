<template>
     <div class="FormBlock">
          <slot></slot>
     </div>
</template>

<script>

export default{
     name: 'form-block',
}

</script>

<style lang="scss" scoped>
     .FormBlock{
          overflow: hidden;
          border-radius: 8px;
          height: 35px;
          max-width: 220px;
          position: relative;
          background: rgba(3, 3, 3, 0.34);
     }

</style>