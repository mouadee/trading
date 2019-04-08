<template>
    <div class="container">
        <div class="row">
            <stock v-for="stock in stocks" :stockProps="stock"></stock>
        </div>
    </div>
</template>



<script>
    import stock from '../components/stocks/stock'
    export default {
        components: {
            stock
        },
        computed: {
            stocks () {
                return this.$store.getters.stocks 
            }
        }
    };
</script>

<style scoped>
    .container {
        padding: 20px;
    }
</style>