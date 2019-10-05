<template>
    <main-layout>
        <h2>如何做一个好看的按钮？</h2>
        <p>技术储备：box-shadow,transform,translate,active,hover</p>
        <h3>1.首先画一个矩形并配上颜色</h3>
        <div class="demo">
            <div class="button1">提交评论</div>
        </div>
        <h3>2.利用box-shadow给button绘制阴影</h3>
        <div class="demo">
            <div class="button2">提交评论</div>
        </div>
        <h3>3.利用hover伪类给button加上移入效果</h3>
        <div class="demo">
            <div class="button3">提交评论</div>
        </div>
        <h3>4.利用active伪类和translate，transform技术给按钮赋予灵魂</h3>
        <div class="demo">
            <div class="button4">提交评论</div>
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
    .button1 {
        background-color: rgb(240, 243, 249);
        width: 400px;
        height: 200px;
        margin: 0 auto;
        display: flex;
        justify-content: center;
        align-items: center;
        border: 1px solid rgb(175, 196, 243);
        cursor: pointer;
    }

    .button2 {
        background-color: rgb(240, 243, 249);
        width: 400px;
        height: 200px;
        margin: 0 auto;
        display: flex;
        justify-content: center;
        align-items: center;
        border: 1px solid rgb(175, 196, 243);
        cursor: pointer;
        box-shadow: 1px 1px 1px rgb(175, 196, 234),
        2px 2px 1px rgb(175, 196, 234),
        3px 3px 1px rgb(175, 196, 234),
        4px 4px 1px rgb(175, 196, 234),
        5px 5px 1px rgb(175, 196, 234),
        6px 6px 1px rgb(175, 196, 234),
        7px 7px 1px rgb(175, 196, 234),
        8px 8px 1px rgb(175, 196, 234);
    }

    .button3 {
        background-color: rgb(240, 243, 249);
        width: 400px;
        height: 200px;
        margin: 0 auto;
        display: flex;
        justify-content: center;
        align-items: center;
        border: 1px solid rgb(175, 196, 243);
        cursor: pointer;
        box-shadow: 1px 1px 1px rgb(175, 196, 234),
        2px 2px 1px rgb(175, 196, 234),
        3px 3px 1px rgb(175, 196, 234),
        4px 4px 1px rgb(175, 196, 234),
        5px 5px 1px rgb(175, 196, 234),
        6px 6px 1px rgb(175, 196, 234),
        7px 7px 1px rgb(175, 196, 234),
        8px 8px 1px rgb(175, 196, 234);

        &:hover {
            background-color: rgb(234, 237, 245);
        }
    }

    .button4 {
        background-color: rgb(240, 243, 249);
        width: 400px;
        height: 200px;
        margin: 0 auto;
        display: flex;
        justify-content: center;
        align-items: center;
        border: 1px solid rgb(175, 196, 243);
        cursor: pointer;
        box-shadow: 1px 1px 1px rgb(175, 196, 234),
        2px 2px 1px rgb(175, 196, 234),
        3px 3px 1px rgb(175, 196, 234),
        4px 4px 1px rgb(175, 196, 234),
        5px 5px 1px rgb(175, 196, 234),
        6px 6px 1px rgb(175, 196, 234),
        7px 7px 1px rgb(175, 196, 234),
        8px 8px 1px rgb(175, 196, 234);

        &:hover {
            background-color: rgb(234, 237, 245);
        }

        &:active {
            box-shadow: 1px 1px 1px rgb(175, 196, 234),
            2px 2px 1px rgb(175, 196, 234),
            3px 3px 1px rgb(175, 196, 234),
            4px 4px 1px rgb(175, 196, 234),
            5px 5px 1px rgb(175, 196, 234);
            transform: translate(3px, 3px);
        }
    }
</style>
