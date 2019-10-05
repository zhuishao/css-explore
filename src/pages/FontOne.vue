<template>
    <main-layout>

            <h2>如何做一个好看的字体?</h2>
            <p>技术储备：linear-gradient, -webkit-background-clip,-webkit-text-fill-color</p>
            <h3>1.先写出最普通的字</h3>
            <div class="demo">
                <p class="text1"><span>Constant dropping wears the stone</span></p>
            </div>
            <h3>2.利用linear-gradient设置线性渐变</h3>
            <div class="demo">
                <p class="text2"><span>Constant dropping wears the stone</span></p>
            </div>
            <h3>3.利用-webkit-background-clip:text将背景剪裁到字体，-webkit-text-fill-color:transparent使字体颜色变成透明</h3>
            <div class="demo">
                <p class="text3"><span>Constant dropping wears the stone</span></p>
            </div>
            <h3>4.使用animation和filter:hue-rotate</h3>
            <div class="demo">
                <p class="text4"><span>Constant dropping wears the stone</span></p>
            </div>
            <h3>5.或使用animation和background-position做一个规律运动的字体</h3>
            <div class="demo">
                <p class="text5"><span>Constant dropping wears the stone</span></p>
            </div>
    </main-layout>
</template>

<script>
    import MainLayout from '../layouts/Main.vue'

    export default {
        components: {
            MainLayout
        },
        mounted() {
            window.scrollTo(0,0);
        }
    }
</script>
<style lang="less" scoped>
    @keyframes pulse {
        from{
            filter: hue-rotate(0);
        }
        to{
            filter: hue-rotate(360deg);
        }
    }
    @keyframes bgp {
       from{
           background-position: 0 0;
       }
        to{
            background-position: -100% 0;
        }
    }
    .text1{
        text-align: center;
    }
    .text2{
        text-align: center;
        background-color: aqua;
        background-image: linear-gradient(to right, red, orange, yellow, green, yellow, orange, red, orange, yellow, green, yellow, orange, red);
    }
    .text3{
        text-align: center;
        -webkit-background-clip: text;
        color:transparent;
        /*-webkit-text-fill-color: transparent;*/
        -webkit-background-size: 200% 100%;
        background-color: aqua;
        background-image: linear-gradient(to right, red, orange, yellow, green, yellow, orange, red, orange, yellow, green, yellow, orange, red);
    }
    .text4{
        .text3;
        animation: pulse 5s infinite;
    }
    .text5{
        .text3;
        animation: bgp 3s infinite;
    }
</style>
