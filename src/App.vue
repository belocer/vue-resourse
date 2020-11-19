<template>
    <div class="container">
        <nav class="navbar navbar-expand-lg navbar-light bg-light">
            <div class="navbar-collapse">
                <ul class="navbar-nav">
                    <router-link tag="li" class="nav-item" exact :to="'/'" active-class="active">
                        <a class="nav-link">Home</a>
                    </router-link>
                    <router-link tag="li" class="nav-item" :to="'/cars'" active-class="active">
                        <a class="nav-link">Cars</a>
                    </router-link>

                    <router-link tag="li" class="nav-item" :to="'/car/3'" active-class="active">
                        <a class="nav-link">Car 3</a>
                    </router-link>
                    <router-link tag="li" class="nav-item" :to="'/car/4'" active-class="active">
                        <a class="nav-link">Car 4</a>
                    </router-link>

                    <router-link tag="li" class="nav-item" :to="'/createCar'" active-class="active">
                        <a class="nav-link">Create car</a>
                    </router-link>
                </ul>
            </div>
        </nav>

        <router-view></router-view>
    </div>
</template>

<script>
  export default {}
</script>

<style scoped>
    .navbar-nav {
        display: flex !important;
        flex-direction: row;
    }

    li {
        margin-right: 20px;
    }
</style>
