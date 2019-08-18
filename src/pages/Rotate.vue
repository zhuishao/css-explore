<template>
    <MainLayout>
        <h2>一个特效</h2>
        <div class="demo2">
            <div class="ray-wrap"></div>
        </div>
    </MainLayout>
</template>

<script>
    import MainLayout from '../layouts/Main.vue'

    export default {
        data() {
            return {
                support: false,
            }
        },
        components: {
            MainLayout
        },
        mounted() {
            window.scrollTo(0, 0);
            this.support = 'clip-path' in document.documentElement.style
            console.log(this.support);
            console.log(document.documentElement.style);
        }
    }
</script>

<style scoped lang="less">
    @keyframes rotate {
        0% {
            transform: rotate(0);
        }
        100% {
            transform: rotate(360deg);
        }
    }

    .ray-wrap {
        width: 50px;
        height: 50px;
        margin: auto;
        position: relative;

        &:before {
            position: absolute;
            content: '';
            top: 0;
            bottom: 0;
            left: 0;
            right: 0;
            clip-path: polygon(50% 0, 55% 45%, 100% 50%, 55% 55%, 50% 100%, 45% 55%, 0 50%, 45% 45%, 50% 0);
            background-image: radial-gradient(rgb(186, 236, 255) 0, rgb(89, 208, 254) 40%, rgb(33, 57, 101) 100%);
            animation: rotate 3s infinite;
            filter:blur(4px) contrast(4);

        }
    }

</style>
