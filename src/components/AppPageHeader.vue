<script>
export default {
    name: 'AppPageHeader',
    props: ['links']
}
</script>

<template>
    <header>
        <div class="sfondo-header">
            <div class="container d-flex justify-content-between pt-3">
                <div class="left pt-2">
                        <p class="text-white d-flex align-items-center gap-2 small">
                            <i class="fa-solid fa-location-dot text-warning"></i>
                            6767 Santa Monica Bivid, Los Angeles, CA 90038
                        </p>
                    <div class="logo">
                        <img src="/src/assets/images/mt-2236-home-logo.png" >
                    </div>
                </div>
                <div class="right">
                    <div class="d-flex justify-content-between">
                            <p class="text-white d-flex gap-2 small align-items-baseline pt-2">
                                <i class="fa-solid fa-phone text-warning"></i>
                                Call Now 123-456-789
                            </p>
                        <button type="button" class="btn btn-light px-5 rounded-3">Donate</button>
                    </div>
                    <nav>
                        <ul class="d-flex gap-3 flex-wrap small">
                            <li :class="{'active': link.active}" v-for="link in links">
                                <a class="text-white" href="#">{{ link.text }}</a>
                            </li>
                        </ul>
                    </nav>
                </div>
            </div>
        </div>
    </header>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

header{
    background-image: url(/src/assets/images/mt-2236-home-bg1.jpg);

    .sfondo-header{
        background-color: rgba($color: #08121f, $alpha: 0.3);
    }

    .logo{
        max-width: 130px;
    }

    button {
        max-height: 35px;
        font-weight: 600;
    }

}

</style>