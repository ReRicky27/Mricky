<!DOCTYPE html>

<html>
<head>
  <title>Clock</title>
  <link rel="stylesheet" type="text/css" href="csclockcodee.css">

</head>
<body bgcolor="background-color: radial-gradient(rgba(255, 200, 0, 1),black);">

<div class="Clock">
<div class="second"></div>
<div class="minute"></div>
<div class="hour"></div>

<div class="one">1</div>
<div class="two">2</div>
<div class="three">3</div>
<div class="four">4</div>
<div class="five">5</div>
<div class="six">6</div>
<div class="seven">7</div>
<div class="eight">8</div>
<div class="nine">9</div>
<div class="ten">10</div>
<div class="eleven">11</div>
<div class="twelve">12</div>

</div>
</body>
</html>

.body{

  text-align: center;

}
.Clock{
  width: 500px;
  height: 500px;
  background: #00FFFF;
  display:inline-block;
  border-radius: 50%;
  border: 10px solid #000;
  padding: 20px;

}

.second, .minute, .hour{
  line-height 45px;
  position: relative;
  transform-origin: bottom;
}



.second{
  height: 250px;
  width: 5px;
  left: 245px;
  background: #00FFFF;
  z-index: 2;
  animation: sec_anim 60s linear infinite;
}

.minute{
  height: 250px;
  width: 10px;
  left: 242.5px;
  background: #000;
  pointer-events: auto
  transform: rotate(-120deg);
  top: -250px;
  z-index: 2;
  animation: sec_anim 30s linear infinite;
}
.hour{
  height: 180px;
  width: 14px;
  left: 240px;
  top: -430px;
  background: #000;
  z-index: 1;
  animation: hour_anim 60000s linear infinite;
}

@keyframes sec_anim{
  from{transform: rotateZ(0deg);}
  to{transform: rotateZ(360deg);}
}

@keyframes min_anim{
  from{transform: rotateZ(0deg);}
  to{transform: rotateZ(360deg);}
}

@keyframes hour_anim{
  from{transform: rotateZ(60deg);}
  to{transform: rotateZ(360deg);}
}

.one, .two, .three, .four, .five, .six, .seven, .eight, .nine, .ten, .eleven, .twelve{
  font-family: arial;
  font-size:  3.7em;
  position: relative;
  color: #black;
  text-shadow: 0 0 10px white;
  z-index: 0;
}


.one{
  top:-648px;
  left: 123px;
}

.two{
  top: -629px;
  left: 192px;
}


.three{
  top:-603px;
  left: 228px;
}

.four{
  top:-564px;
  left: 203px;
}

.five{
  top:-552px;
  left: 116px;
}

.six{
  top:-580px;
}

.seven{
  top:-691px;
  left: -116px;
}

.eight{
  top:-840px;
  left: -203px;
}

.nine{
  top:-1016px;
  left: -238px;
}

.ten{
  top:-1181px;
  left: -192px;
}

.eleven{
  top:-1338px;
  left: -123px;

}

.twelve{
  top:-1450px;

}
