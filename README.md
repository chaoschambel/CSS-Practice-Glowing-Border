# CSS-Practice-Glowing-Border

body{
    padding: 0;
    margin: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    background: #060c21;
    min-height: 100vh;
}
.box{
    height: 400px;
    width: 300px;
    display: flex;
    align-items: center;
    justify-content: center;
    position: relative;
    background: #060c21;
}
.box::before{
    content: '';
    top: -2px;
    right: -2px;
    bottom: -2px;
    left: -2px;
    position: absolute;
    background: #fff;
    z-index: -1;
}
.box::after{
    content: '';
    top: -2px;
    right: -2px;
    bottom: -2px;
    left: -2px;
    position: absolute;
    background: #fff;
    z-index: -2;
    filter: blur(40px);
}
.box::before,.box::after{
    background: linear-gradient(235deg, rgb(51, 202, 51), #060c21, rgb(108, 108, 204));
}
.content{
    padding: 20px;
    color: #fff;
    box-sizing: border-box;
}
