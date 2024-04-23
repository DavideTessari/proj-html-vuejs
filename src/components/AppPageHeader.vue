<script>
export default {
    name: 'AppPageHeader',
    props: ['links']
}
</script>

<template>
    <header>
        <nav>
            <ul>
                <li :class="{'active': link.active}" v-for="link in links">
                    <a href="#">{{ link.text }}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

</style>