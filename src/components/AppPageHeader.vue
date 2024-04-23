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
                                <a class="" href="#">{{ link.text }}</a>
                            </li>
                        </ul>
                    </nav>
                </div>
            </div>
        </div>
        <div class="container">
            <section class="col-lg-6">
                <span class="badge text-bg-warning py-0">Welcome</span>
                <h1 class="text-white fw-bold pt-3">ACADEMIC CHESS FOR <p class="yellow">EVERYONE</p></h1>
                <p class="medium text-white">Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptates nihil, ratione voluptate saepe quod voluptatum quibusdam totam error aperiam quo voluptas optio blanditiis eaque asperiores placeat accusamus corporis unde ipsam.</p>
            
                <div class="d-flex gap-3 pt-3">
                    <button type="button" class="btn medium fw-bold px-4">Email Now</button>
                    <button type="button" class="btn btn-outline-light medium fw-bold px-4">Learn More</button>
                </div>
            </section>
        </div>
    </header>
</template>


<style scoped lang="scss">
@use '../style/partials/variables' as *;

header {
    background-image: url('/src/assets/images/mt-2236-home-bg1.jpg');

    .sfondo-header{
        background-color: rgba($color: #08121f, $alpha: 0.3);

        .logo{
            max-width: 130px;
        }

        button {
            max-height: 35px;
            font-weight: 600;
        }

        li a:first-child {
            color: white !important;
        }
    }

    section{
        padding: 80px 0;

        .badge{
            font-size: 11px;
            font-weight: 100;
        }

        h1 p{
            color: $yellow;
        }

        h1 {
            font-size: 45px;
        }

        button:first-child{
            background-color: $yellow;
        }
    }
}
</style>

