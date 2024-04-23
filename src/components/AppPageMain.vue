<script>
export default {
    name: 'AppPageMain',
}
</script>

<template>
    <main>
        <div class="container py-5">
            <h2 class="text-center fw-bold fs-4 lh-1">OUR SERVICES</h2>
            <p class="text-center medium lh-1 py-2">We make your child happy day after day</p>
            <div class="d-flex gap-5">
                <div class="col-4">
                    <p class="fw-bold">Chess Education</p>
                    <p class="small">Popular education for your child and you</p>
                    <p class="smaller">Lorem ipsum, dolor sit amet consectetur adipisicing elit. A placeat necessitatibus, tempore, reprehenderit aperiam earum quod cumque corporis itaque voluptatum architecto perferendis, hic fugiat dolor iure fuga nam adipisci officia.</p>
                    <div class="d-flex lh-1">
                        <div class="bullett-icon px-2">
                            <img src="/src/assets/images/mt-2236-home-icon-bullet.png" alt="scacco">
                        </div>
                        <p class="smaller">Build self regulation and motivation</p>
                    </div>
                    <div class="d-flex lh-1">
                        <div class="bullett-icon px-2">
                            <img src="/src/assets/images/mt-2236-home-icon-bullet.png" alt="scacco">
                        </div>
                        <p class="smaller">Build self regulation and motivation</p>
                    </div>
                    <div class="d-flex lh-1">
                        <div class="bullett-icon px-2">
                            <img src="/src/assets/images/mt-2236-home-icon-bullet.png" alt="scacco">
                        </div>
                        <p class="smaller">Build self regulation and motivation</p>
                    </div>
                    <div class="d-flex lh-1">
                        <div class="bullett-icon px-2">
                            <img src="/src/assets/images/mt-2236-home-icon-bullet.png" alt="scacco">
                        </div>
                        <p class="smaller">Build self regulation and motivation</p>
                    </div>
                    <div class="d-flex lh-1">
                        <div class="bullett-icon px-2">
                            <img src="/src/assets/images/mt-2236-home-icon-bullet.png" alt="scacco">
                        </div>
                        <p class="smaller">Build self regulation and motivation</p>
                    </div>
                </div>
                <div class="col-4">
                    <div class="icon-home">
                        <img src="/src/assets/images/mt-2236-home-icon1.png">
                    </div>
                        <p class="fw-bold pt-3 medium">Various Age Groups</p>
                        <p class="smaller">Lorem ipsum dolor sit amet consectetur adipisicing elit.iatur error facilis!</p>
                    <div class="icon-home pt-4">
                        <img src="/src/assets/images/mt-2236-home-icon3.png">
                    </div>
                        <p class="fw-bold pt-3 medium">Best Chess Players</p>
                        <p class="smaller">Lorem ipsum dolor sit amet consectetur adipisicing elit.iatur error facilis!</p>
                    </div>
                <div class="col-4">
                    <div class="icon-home">
                        <img src="/src/assets/images/mt-2236-home-icon2.png">
                    </div>
                        <p class="fw-bold pt-3 medium">Top Chess Variants</p>
                        <p class="smaller">Lorem ipsum dolor sit amet consectetur adipisicing elit.iatur error facilis!</p>
                    <div class="icon-home pt-4">
                        <img src="/src/assets/images/mt-2236-home-icon4.png">
                    </div>
                        <p class="fw-bold pt-3 medium">Best Chess Openings</p>
                        <p class="smaller">Lorem ipsum dolor sit amet consectetur adipisicing elit.iatur error facilis!</p>
                </div>
            </div>
            <button type="button" class="btn medium fw-bold px-4 mt-4">Learn More</button>
        </div>
        
    </main>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

main {

    p{
        color: $dark-grey;
    }

    .icon-home {
        max-width: 40px;
    }

    button{
            background-color: $yellow;
        }
}

</style>
