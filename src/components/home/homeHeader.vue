<template>
    <nav class="navbar navbar-expand-lg navbar-light bg-light">
        <router-link to="/" class="navbar-brand">Trading</router-link>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav mr-auto">
                <router-link class="nav-link" to="/portfolio" tag="li" active-class="active">Portfolio</router-link>
                <router-link class="nav-link" to="/stocks" tag="li" active-class="active">Stocks</router-link>

                <li class="nav-link float-right">End Day</li>
                <li class="nav-item dropdown">
                    <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                        Save | Load
                    </a>
                    <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                        <a class="dropdown-item" href="#">Save data</a>
                        <a class="dropdown-item" href="#">Load Data</a>
                    </div>
                </li>
            </ul>
        </div>
    </nav>
</template>

<script>
    export default {
        name: "homeHeader"
    }
</script>

<style scoped>

</style>