<template>
    <main-layout>
        <div class="demo">
            <div class="bl">
                <div class="t"></div>
                <div class="t"></div>
                <div class="t"></div>
                <div class="t"></div>
                <div class="t"></div>
                <div class="t"></div>
            </div>
        </div>
        <hr>
        <div class="demo2">
            <div class="line-left"></div>
            <div class="triL"></div>
            <div class="line-center"></div>
            <div class="triR"></div>
            <div class="line-right"></div>
        </div>
        <div class="demo">
            <div class="text"></div>
        </div>
    </main-layout>
</template>

<script>
    import MainLayout from '../layouts/Main.vue'
    export default {
        components: {
            MainLayout
        },
        name: "triangleMove"
    }
</script>

<style scoped lang="less">
    @keyframes triMove1 {
        0%{
            /*transform:rotate(45deg) translate(0,0);*/
            /*filter:drop-shadow(2px 0 4px 4px #fff) blur(0) contrast(0);*/
            opacity: .4;
        }
        15%{
            opacity: 1;
            filter: brightness(200%) drop-shadow(0 0 20px #fff);
        }
        16%{
            opacity: .4;
        }
        100%{
            opacity: .4;
            /*transform:rotate(45deg) translate(123px,-123px);*/
            /*filter:drop-shadow(2px 0 4px 4px #fff) blur(3px) contrast(20);*/
        }
    }
    @keyframes triMove2 {
        0%{
            opacity: .4;
            /*transform:rotate(45deg) translate(0,0);*/
            /*border-color: blueviolet;*/
        }
        15%{
            opacity: .4;
        }
        30%{
            opacity: 1;
            filter: brightness(200%) drop-shadow(0 0 20px #fff);
        }
        31%{
            opacity: .4;
        }
        100%{
            opacity: .4;
            /*transform: rotate(45deg) translate(123px,-123px);*/
        }
    }
    @keyframes triMove3 {
        0%{
            /*transform:rotate(45deg) translate(0,0);*/
            /*border-color: blueviolet;*/
            opacity: .4;
        }
        30%{
            opacity: .4;
        }
        45%{
            filter: brightness(200%) drop-shadow(0 0 20px #fff);
            opacity: 1;
        }
        46%{
            opacity: .4;
        }
        100%{
            opacity: .4;
            /*transform:rotate(45deg) translate(123px,-123px);*/
        }
    }
    @keyframes triMove4 {
        0%{
            /*transform:rotate(45deg) translate(0,0);*/
            /*border-color: blueviolet;*/
            opacity: .4;
        }
        45%{
            opacity: .4;
        }
        60%{
            filter: brightness(200%) drop-shadow(0 0 20px #fff);
            opacity: 1;
        }
        61%{
            opacity: .4;
        }
        100%{
            opacity: .4;
            /*transform:rotate(45deg) translate(123px,-123px);*/
        }
    }
    @keyframes triMove5 {
        0%{
            /*transform:rotate(45deg) translate(0,0);*/
            /*filter:drop-shadow(2px 0 4px 4px #fff) blur(0) contrast(0);*/
            opacity: .4;
        }
        60%{
            opacity: .4;
        }
        75%{
            filter: brightness(200%) drop-shadow(0 0 20px #fff);
            opacity: 1;
        }
        76%{
            opacity: .4;
        }
        100%{
            opacity: .4;
            /*transform:rotate(45deg) translate(123px,-123px);*/
            /*filter:drop-shadow(2px 0 4px 4px #fff) blur(3px) contrast(20);*/
        }
    }
    @keyframes triMove6 {
        0%{
            opacity: .4;
            /*transform:rotate(45deg) translate(0,0);*/
            /*border-color: blueviolet;*/
        }
        75%{
            opacity: .4;
        }
        90%{
            filter: brightness(200%) drop-shadow(0 0 20px #fff);
            opacity: 1;
        }
        91%{
            opacity: .4;
        }
        100%{
            opacity: .4;
            /*transform: rotate(45deg) translate(123px,-123px);*/
        }
    }

    @keyframes flow1 {
        0%{
            background-position: 0;
        }
        30%{
            background-position: -122%;
        }
        100%{
            background-position: -122%;
        }
    }
    @keyframes flow2 {
        0%{
            background-position: 0;
        }
        10%{
            background-position: 0;
        }
        40%{
            background-position: -122%;
        }
        100%{
            background-position: -122%;
        }
    }
    @keyframes flow3 {
        0%{
            background-position: 0;
        }
        20%{
            background-position: 0;
        }
        60%{
            background-position: -122%;
        }
        100%{
            background-position: -122%;
        }
    }
    @keyframes flow4 {
        0%{
            background-position: 0;
        }
        30%{
            background-position: 0;
        }
        90%{
            background-position: -122%;
        }
        100%{
            background-position: -122%;
        }
    }
    @keyframes flow5 {
        0%{
            background-position: 0;
        }
        40%{
            background-position: 0;
        }
        100%{
            background-position: -122%;
        }

    }

    .bl{
        background-color: rgb(9,5,19);
        overflow: hidden;
        width: 200px;
        height: 50px;
        border-width: 5px 0;
        border-style: dashed;
        color:#1E73FF;
        position: relative;
        .t{
            top: 13px;
            position: absolute;
            border-radius: 2px;
            width: 20px;
            height: 20px;
            border-width: 5px 5px 0 0;
            border-style: solid;
            transform: rotate(45deg);
            border-color: rgb(0,85,255);
            &:nth-of-type(1){
                left: 20px;
                animation: triMove1 5s infinite;
            }
            &:nth-of-type(2){
                left: 40px;
                animation: triMove2 5s infinite;
            }
            &:nth-of-type(3){
                left: 60px;
                animation: triMove3 5s infinite;
            }
            &:nth-of-type(4){
                left: 100px;
                opacity: .4;
                animation: triMove4 5s infinite;
            }
            &:nth-of-type(5){
                left: 120px;
                opacity: .4;
                animation: triMove5 5s infinite;
            }
            &:nth-of-type(6){
                left: 140px;
                opacity: .4;
                animation: triMove6 5s infinite;
            }
        }

    }
    .line-left{
        position: absolute;
        left: 0;
        width: 200px;
        height: 4px;
        background-image: linear-gradient(to right, rgb(6,3,19) 0, rgb(17,47,92) 50%, #1374bd 70%, #00c8ff 90%, #0d1732 95%, #0d1732 200%);
        background-size: 300%;
        animation: flow1 3s infinite;
    }
    .triL{
        position: absolute;
        left: 192px;
        margin-top:13px;
        width: 40px;
        height: 4px;
        background-image: linear-gradient(to right, rgb(17,47,92) 0, rgb(19,59,110) 50%, #1374bd 70%, #00c8ff 90%, #0d1732 95%, #0d1732 200%);
        background-size: 300%;
        transform: rotate(45deg);
        background-color: aquamarine;
        border-radius: 2px;
        animation: flow2 3s infinite;
    }
    .triR{
        position: absolute;
        right: 192px;
        margin-top:13px;
        width: 40px;
        height: 4px;
        background-image: linear-gradient(to right, #0d1732 0, #0d1732 50%, #1374bd 70%, #00c8ff 90%, #0d1732 95%, #0d1732 200%);
        background-size: 300%;
        transform: rotate(-45deg);
        background-color: aquamarine;
        border-radius: 2px;
        animation: flow4 3s infinite;
    }
    .line-center{
        position: absolute;
        height: 4px;
        background-image: linear-gradient(to right,rgb(19,59,110) 0, rgb(0,193,255) 15%,rgb(19,59,110) 30%, #1374bd 70%, #00c8ff 90%, #0d1732 95%, #0d1732 200%);
        background-size: 300%;
        right: 224px;
        left: 224px;
        margin-top:26px;
        background-color: aqua;
        animation: flow3 3s infinite;
    }
    .line-right{
        position: absolute;
        background-image: linear-gradient(to right, #0d1732 0, #0d1732 50%, #1374bd 70%, #00c8ff 90%, #0d1732 95%, #0d1732 200%);
        background-size: 300%;
        right: 0;
        width: 200px;
        height: 4px;
        background-color: aquamarine;
        animation: flow5 3s infinite;
    }
    .text{
        height: 20px;
        transform: skewX(-30deg);
        background-image: linear-gradient(to right,black 0,black 8%,transparent 8%,transparent 10%,black 10%,black 18%,transparent 18%,transparent 20%,black 20%,black 28%,transparent 28%,transparent 30%,black 30%,black 38%,transparent 38%,transparent 40%,black 40%,black 48%,transparent 48%,transparent 50%,black 50% ,black 60%,transparent 60%,black 70%,transparent 70%,black 80%,transparent 80%,black 90%,transparent 90%,black 100%);
    }
</style>
