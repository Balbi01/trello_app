<template>
    <footer>
        <span style="margin:5px;">
            Desarrollado con ❤️
            <!-- <svg 
                xmlns="http://www.w3.org/2000/svg" 
                width="24" 
                height="24" 
                viewBox="0 0 24 24" 
                fill="none" 
                stroke="currentColor" 
                stroke-width="2" 
                stroke-linecap="round" 
                stroke-linejoin="round" 
                class="lucide lucide-heart css-1yx1qo4">
                <path d="M19 14c1.49-1.46 3-3.21 3-5.5A5.5 5.5 0 0 0 16.5 3c-1.76 0-3 .5-4.5 2-1.5-1.5-2.74-2-4.5-2A5.5 5.5 0 0 0 2 8.5c0 2.3 1.5 4.05 3 5.5l7 7Z">
                </path>
            </svg> -->
            &amp; <span><a style="text-decoration: none;" href="//vuejs.org">Vue.js</a></span>
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