<template>
    <footer>
        <span style="margin:5px;">
            Desarrollado con ❤️ &amp; <span><a style="text-decoration: none;" href="//vuejs.org">Vue.js</a></span>
            desde México

        </span>
    </footer>
</template>

<script>
const AppFooter = {
    name: 'app-footer'
}

export default AppFooter;
</script>

<style lang="scss" scoped>
    footer {
        box-sizing: border-box;
        background-color: #cfd8dc;
        bottom: 0;
        left: 0;
        padding: 1rem;
        position: absolute;
        width: 100%;
    }
    a {
        color: #546E7A;
    }
</style>