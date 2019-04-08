<template>
    <div class="container">
      <div class="row">
        <div class="col-12">
          <homeHeader></homeHeader>
          <router-view></router-view>
        </div>
      </div>
    </div>
</template>
<script>
  import homeHeader from './components/home/homeHeader'
  export default {
    components: {
      homeHeader,
    },
    created() {
        this.$store.dispatch('setStocks')
    }
  }
</script>

<style scoped>
 .container {
   padding: 0;
   margin: unset
 }
</style>
