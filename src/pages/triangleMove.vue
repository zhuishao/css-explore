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
        <div class="demo">
            <div class="flow-x">
                <div v-for="k in 9" class="flow-x-ar" :key="k"></div>
            </div>
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
            left: 20px;
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
            left: 200px;
            /*transform:rotate(45deg) translate(123px,-123px);*/
            /*filter:drop-shadow(2px 0 4px 4px #fff) blur(3px) contrast(20);*/
        }
    }
    @keyframes triMove2 {
        0%{
            opacity: .4;
            left: 40px;
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
            left: 220px;
            /*transform: rotate(45deg) translate(123px,-123px);*/
        }
    }
    @keyframes triMove3 {
        0%{
            /*transform:rotate(45deg) translate(0,0);*/
            /*border-color: blueviolet;*/
            opacity: .4;
            left: 60px;
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
            left: 240px;
            /*transform:rotate(45deg) translate(123px,-123px);*/
        }
    }
    @keyframes triMove4 {
        0%{
            /*transform:rotate(45deg) translate(0,0);*/
            /*border-color: blueviolet;*/
            opacity: .4;
            left: 100px;
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
            left: 280px;
            /*transform:rotate(45deg) translate(123px,-123px);*/
        }
    }
    @keyframes triMove5 {
        0%{
            /*transform:rotate(45deg) translate(0,0);*/
            /*filter:drop-shadow(2px 0 4px 4px #fff) blur(0) contrast(0);*/
            opacity: .4;
            left: 120px;
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
            left: 300px;
            /*transform:rotate(45deg) translate(123px,-123px);*/
            /*filter:drop-shadow(2px 0 4px 4px #fff) blur(3px) contrast(20);*/
        }
    }
    @keyframes triMove6 {
        0%{
            left: 140px;
            opacity: .4;
            /*transform:rotate(45deg) translate(0,0);*/
            /*border-color: blueviolet;*/
        }
        75%{
            opacity: .4;
        }
        50%{
            left: 320px;
        }
        90%{
            filter: brightness(200%) drop-shadow(0 0 20px #fff);
            opacity: 1;
        }
        91%{
            opacity: .4;
        }
        100%{
            left: 320px;
            opacity: .4;
            /*transform: rotate(45deg) translate(123px,-123px);*/
        }
    }

    @keyframes flow1 {
        0% {
        }
        15%{
            left: 100%;
        }
        100%{
            left: 100%;
            background-image: linear-gradient(to right,rgb(0,244,255),rgb(0,244,255));
        }
    }
    @keyframes flow2 {
        5%{
            left: -100px;
        }
        12%{
            left: 100%;
        }
        100%{
            left: 100%;
        }
    }
    @keyframes flow3 {
        7%{
            left: -100px;
        }
        66%{
            left: 100%;
        }
        100%{
            left: 100%;
        }
    }
    @keyframes flow4 {
        45%{
            left: -100px;
        }
        70%{
            left: 100%;
        }
        100%{
            left: 100%;
        }
    }
    @keyframes flow5 {
        50%{
            left: -100px;
        }
        90%{
            left: 100%;
        }
        100%{
            left: 100%;
        }

    }

    @keyframes ar-m-1 {
       0%{
           transform: translateX(-900%) rotate(45deg);
           opacity: .3;
       }
        100%{
            opacity: .3;
            transform: translateX(-400%) rotate(45deg);
        }
    }
    @keyframes ar-m-2 {
        0%{
            opacity:.3;
            transform: translateX(-750%) rotate(45deg);
        }
        100%{
            opacity:.4;
            transform: translateX(-250%) rotate(45deg);
        }
    }
    @keyframes ar-m-3 {
        0%{
            opacity:.3;
            transform: translateX(-600%) rotate(45deg);
        }
        33%{
            opacity: .3;
        }
        100%{
            opacity: .8;
            transform: translateX(-100%) rotate(45deg);
        }
    }
    @keyframes ar-m-4 {
        0%{
            opacity: .3;
            transform: translateX(-400%) rotate(45deg);
        }
        66%{
            opacity: .8;
        }
        82%{
            opacity: 1;
        }
        100%{
            opacity: .8;
            transform: translateX(100%) rotate(45deg);
        }
    }
    @keyframes ar-m-5 {
        0%{
            opacity: .4;
            transform: translateX(-250%) rotate(45deg);
        }
        50%{
            opacity: 1;
        }
        100%{
            opacity: .4;
            transform: translateX(250%) rotate(45deg);
        }
    }
    @keyframes ar-m-6 {
        0%{
            opacity: .8;
            transform: translateX(-100%) rotate(45deg);
        }
        16%{
            opacity: 1;
        }
        100%{
            opacity:.3;
            transform: translateX(400%) rotate(45deg);
        }
    }
    @keyframes ar-m-7 {
        0%{
            opacity: .8;
            transform: translateX(100%) rotate(45deg);
        }
        66%{
            opacity: .3;
        }
        100%{
            opacity:.3;
            transform: translateX(600%) rotate(45deg);
        }
    }
    @keyframes ar-m-8 {
        0%{
            opacity: .4;
            transform: translateX(250%) rotate(45deg);
        }
        100%{
            opacity:.3;
            transform: translateX(750%) rotate(45deg);
        }
    }
    @keyframes ar-m-9 {
        0%{
            opacity:.3;
            transform: translateX(400%) rotate(45deg);
        }
        100%{
            opacity:.3;
            transform: translateX(900%) rotate(45deg);
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
        background-image: linear-gradient(to right, rgb(6,3,19) 0, rgb(17,47,92));
        overflow: hidden;
        &:before{
            content: '';
            position: absolute;
            top: 0;
            bottom: 0;
            left: -100px;
            width: 100px;
            background-image: linear-gradient(to right,transparent,rgb(0,244,255));
            animation: flow1 6s infinite;
            border-radius:5px;
        }
    }
    .triL{
        position: absolute;
        left: 192px;
        margin-top:13px;
        width: 40px;
        height: 4px;
        background-image: linear-gradient(to left,rgb(20,72,130),rgb(17,47,91));
        transform: rotate(45deg);
        background-color: aquamarine;
        border-radius: 2px;
        overflow: hidden;
        &:before{
            content: '';
            position: absolute;
            top: 0;
            bottom: 0;
            left: -100px;
            width: 100px;
            animation: flow2 6s infinite;
            background-image: linear-gradient(to right,transparent,rgb(0,244,255));
            border-radius:5px;
        }
    }
    .triR{
        position: absolute;
        right: 192px;
        margin-top:13px;
        width: 40px;
        height: 4px;
        background-image: linear-gradient(to right,rgb(20,72,130),rgb(17,47,91));
        transform: rotate(-45deg);
        background-color: aquamarine;
        border-radius: 2px;
        overflow: hidden;
        &:before{
            content: '';
            position: absolute;
            top: 0;
            bottom: 0;
            left: -100px;
            width: 100px;
            animation: flow4 6s infinite;
            background-image: linear-gradient(to right,transparent,rgb(0,244,255));
            border-radius:5px;
        }
    }
    .line-center{
        position: absolute;
        height: 4px;
        background-image: linear-gradient(to right,rgb(20,72,130) , rgb(0,191,255) ,rgb(20,72,130));
        right: 224px;
        left: 224px;
        margin-top:26px;
        background-color: aqua;
        overflow: hidden;
        &:before{
            content: '';
            position: absolute;
            top: 0;
            bottom: 0;
            left: -100px;
            border-radius:5px;
            width: 100px;
            animation: flow3 6s infinite;
            background-image: linear-gradient(to right,transparent,rgb(0,244,255));
        }
    }
    .line-right{
        position: absolute;
        background-image: linear-gradient(to right, rgb(17,47,92),rgb(6,3,19));
        right: 0;
        width: 200px;
        height: 4px;
        background-color: aquamarine;
        overflow: hidden;
        &:before{
            content: '';
            position: absolute;
            top: 0;
            bottom: 0;
            left: -100px;
            width: 100px;
            border-radius: 5px;
            animation: flow5 6s infinite;
            background-image: linear-gradient(to right,transparent,rgb(0,244,255));
        }
    }
    .text{
        height: 20px;
        transform: skewX(-30deg);
        background-image: linear-gradient(to right,black 0,black 8%,transparent 8%,transparent 10%,black 10%,black 18%,transparent 18%,transparent 20%,black 20%,black 28%,transparent 28%,transparent 30%,black 30%,black 38%,transparent 38%,transparent 40%,black 40%,black 48%,transparent 48%,transparent 50%,black 50% ,black 60%,transparent 60%,black 70%,transparent 70%,black 80%,transparent 80%,black 90%,transparent 90%,black 100%);
    }
    .flow-x{
        width: 96px;
        height: 15px;
        position: relative;
        overflow: hidden;
        border-style: dashed;
        border-width: 1px 0;
        color: rgb(29,110,245);
    }
    .flow-x-ar{
        width: 8%;
        height: 49%;
        border-width: 2px 2px 0 0;
        border-style: solid;
        border-color: rgb(29,110,245);
        margin: auto;
        position: absolute;
        top:0;
        right: 0;
        left: 0;
        bottom: 0;
        transform: rotate(45deg) translate3d(0,0,0);
        &:nth-of-type(1){
            transform: translateX(-900%) rotate(45deg);
            animation: ar-m-1 2s linear infinite;
        }
        &:nth-of-type(2){
            transform: translateX(-750%) rotate(45deg);
            animation: ar-m-2 2s linear infinite;
        }
        &:nth-of-type(3){
            transform: translateX(-600%) rotate(45deg);
            animation: ar-m-3 2s linear infinite;
        }
        &:nth-of-type(4){
            transform: translateX(-400%) rotate(45deg);
            animation: ar-m-4 2s linear infinite;
        }
        &:nth-of-type(5){
            transform: translateX(-250%) rotate(45deg);
            animation: ar-m-5 2s linear infinite;
        }
        &:nth-of-type(6){
            transform: translateX(-100%) rotate(45deg);
            animation: ar-m-6 2s linear infinite;
        }
        &:nth-of-type(7){
            transform: translateX(100%) rotate(45deg);
            animation: ar-m-7 2s linear infinite;
        }
        &:nth-of-type(8){
            transform: translateX(250%) rotate(45deg);
            animation: ar-m-8 2s linear infinite;
        }
        &:nth-of-type(9){
            transform: translateX(400%) rotate(45deg);
            animation: ar-m-9 2s linear infinite;
        }
    }
</style>
