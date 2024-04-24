<script>
export default {
    name: 'AppPageFooter',
    props: {
        icons: Array,
        copyright: String,
    }
}
</script>

<template>
    <footer>
        <div class="background-darkgrey py-5">
            <div class="container">
                <div class="d-flex justify-content-between ">
                    <div class="d-flex flex-column justify-content-between">
                        <div class="logo">
                            <img src="/src/assets/images/mt-2236-home-logo.png" >
                        </div>
                        <div class="small text-white">{{ copyright }}</div>
                    </div>
                    <div>
                        <p class="text-white medium">Follow Us</p>
                        <nav>
                            <ul class="d-flex gap-2 ">
                                <li v-for="icon in icons" :key="icon.text">
                                    <a class="text-white rounded box" :href="icon.link" v-html="icon.text"></a>
                                </li>
                            </ul>
                        </nav>
                    </div>
                    <div>
                        <p class="small text-white">Subscribe to get the latest news, course updates, discounts, events.</p>
                        <input type="text" class="form-control rounded-0 small" id="formGroupExampleInput" placeholder="Enter your e-mail here">
                        <button type="button" class="btn medium rounded-1 fw-bold px-4 mt-3">Subscribe</button>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

.background-darkgrey{
    background-color: $dark-grey;

    .box {
        display: inline-block;
        border: 1px solid white;
        padding: 8px;
        width: 40px;
        height: 40px;
        text-align: center;
        cursor: pointer;
    }

    button{
        background-color: $yellow;
    }

    
    ul {
        margin: 0;
        padding: 0;
        list-style: none;
    }
}

</style>