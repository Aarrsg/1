<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>安徽站</title>
    <style>
        * {
            padding: 0;
            margin: 0;
            box-sizing: border-box;
        }

        body {
            /* width: 100vw;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center; */
            background-image: linear-gradient(to top, #c6dace 0%, #ffffff 100%);
        }

        .shell {
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .card {
            width: 300px;
            height: 250px;
            position: relative;
            display: flex;
            justify-content: center;
            align-items: flex-end;
            padding: 0 25px;
            perspective: 2500px;
            transition: all 0.4s;
            margin: 0 100px;
        }

        .cover-image {
            width: 100%;
            height: 100%;
        }

        .wrapper {
            transition: all 0.3s;
            position: absolute;
            width: 100%;
            z-index: -1;
        }

        .card:hover .wrapper {
            transform: perspective(900px) translateY(-5%) rotateX(25deg) translateZ(0);
            box-shadow: 2px 35px 32px -8px rgba(0, 0, 0, 0.75);
        }

        .wrapper::before,
        .wrapper::after {
            content: "";
            opacity: 0;
            width: 100%;
            height: 80px;
            transition: all 0.3s;
            position: absolute;
            left: 0;
        }

        .wrapper::before {
            top: 0;
            height: 100%;
            background-image: linear-gradient(to top,
                    transparent 46%,
                    rgba(12, 13, 19, 0.5) 68%,
                    rgba(12, 13, 19) 97%);
        }

        .wrapper::after {
            bottom: 0;
            opacity: 1;
            background-image: linear-gradient(to bottom,
                    transparent 46%,
                    rgba(12, 13, 19, 0.5) 68%,
                    rgba(12, 13, 19) 97%);
        }

        .card:hover .wrapper::before,
        .wrapper::after {
            opacity: 1;
        }

        .card:hover .wrapper::after {
            height: 200px;
        }

        .title {
            width: 100%;
            transition: transform 0.3s;
        }

        .card:hover .title {
            transform: translate3d(0%, -50px, 100px);
        }

        .character {
            width: 100%;
            opacity: 0;
            transition: all 0.3s;
            position: absolute;
            z-index: -1;
        }

        .card:hover .character {
            opacity: 1;
            transform: translate3d(0%, -20%, 100px);
        }

        .card:hover {
            transform: translateY(40px);
        }

        .img img {
            width: 100%;
            object-fit: contain;
        }

        .section {
            display: flex;
        }

        .section-1 {
            width: 800px;
            height: 300px;
            margin: 60px auto;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            border: 1px solid #ccc;
        }

        .section-2 {
            width: 800px;
            margin: 60px auto;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .section-2 .img {
            width: 40%;
        }

        .section-3 {
            width: 800px;
            margin: 60px auto;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .section-3 .img {
            width: 50%;
        }

        .section-3 .content {
            width: 50%;
            text-align: center;
        }
    </style>
</head>

<body>
    <div class="section section-1">
        <p>安徽站</p>
    </div>
    <!-- <div class="section section-2">
        <div class="img">
            <img src="./image/01.png" alt="">
        </div>
        <div class="img">
            <img src="./image/01.png" alt="">
        </div>
    </div> -->
    <div class="shell">
        <div class="card">
            <div class="wrapper">
                <img src="./image/01.png" alt="" class="cover-image">
            </div>
            <img src="./image/02.png" alt="" class="character">
        </div>

        <div class="card">
            <div class="wrapper">
                <img src="./image/01.png" alt="" class="cover-image">
            </div>
            <img src="./image/04.png" alt="" class="character">
        </div>
    </div>
    <div class="section section-3">
        <div class="img">
            <img src="./image/05.png" alt="">
        </div>
        <div class="content">
            宏村：一生痴绝处，无梦到徽州。宏村，一幅流动的水墨画卷，
        青瓦白墙间诉说着千年的故事。湖光山色映古韵，四季皆景入诗篇。
        </div>
    </div>
    <div class="section section-3">
        <div class="content">
            黄山：安徽有着江南的温婉，更带着历史的浑厚和沉淀。五岳归
        来不看山，只看黄山不看岳。
        </div>
        <div class="img">
            <img src="./image/5.jpg" alt="">
        </div>
    </div>
    

</body>

</html>
