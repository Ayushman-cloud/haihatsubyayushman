
<html>
  <body>
    <style>
    $size: 50px;
$xmove: 44.6px;
$ymove: 25.8px;
$shadowfull: 99%;
$rotate-skew: rotate(-45deg) skew(15deg, 15deg);

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background: #00ca92;
}

.container {
  height: 160px;
  width: 160px;
  transform: translate(50%, 10%);

  .cube {
    animation-duration: 0.75s;
    animation-timing-function: linear;
    animation-iteration-count: infinite;

    & > div {
      width: $size;
      height: $size;
      position: absolute;
    }

    .top {
      background: #fff;
      transform: $rotate-skew;
    }

    .left {
      background: #d8d8d8;
      transform: rotate(15deg) skew(15deg, 15deg) translate(-50%, 100%);
    }

    .right {
      background: #c5c5c5;
      transform: rotate(-15deg) skew(-15deg, -15deg) translate(50%, 100%);
    }

    &:nth-child(1) {
      animation-name: anim-one;
    }

    &:nth-child(2) {
      animation-name: anim-two;
    }

    &:nth-child(3) {
      animation-name: anim-three;
    }

    &:nth-child(4) {
      animation-name: anim-four;
    }
  }

  .shadow {
    position: absolute;
    top: 100%;

    & > * {
      display: inline-block;
      background: #006d4f;
      height: 40px;
      width: 40px;
      position: absolute;
      animation-duration: 0.75s;
      animation-timing-function: linear;
      animation-iteration-count: infinite;
    }

    .one {
      animation-name: shadow-one;
    }

    .two {
      animation-name: shadow-two;
    }

    .three {
      animation-name: shadow-three;
    }

    .four {
      animation-name: shadow-four;
    }
  }
}

@keyframes anim-one {
  from {
    transform: translate(-$xmove * 2, 0);
  }
  50% {
    transform: translate(-$xmove, -$ymove);
  }
  to {
    transform: translate(0, 0);
  }
}

@keyframes anim-two {
  from {
    transform: translate(0, 0);
  }
  50% {
    transform: translate(0, 0);
  }
  to {
    transform: translate($xmove, $ymove);
  }
}

@keyframes anim-three {
  from {
    transform: translate(-$xmove, $ymove);
  }
  50% {
    transform: translate(-$xmove, $ymove);
  }
  to {
    transform: translate(-$xmove * 2, 0px);
  }
}

@keyframes anim-four {
  from {
    transform: translate($xmove, $ymove);
  }
  50% {
    transform: translate(0, $ymove * 2);
  }
  to {
    transform: translate(-$xmove, $ymove);
  }
}

@keyframes shadow-one {
  from {
    transform: $rotate-skew translate(-$shadowfull, 0);
  }

  50% {
    transform: $rotate-skew translate(0, 0);
  }

  to {
    transform: $rotate-skew translate(0, $shadowfull);
  }
}

@keyframes shadow-two {
  from {
    transform: $rotate-skew translate(-$shadowfull, $shadowfull);
  }

  50% {
    transform: $rotate-skew translate(-$shadowfull, $shadowfull);
  }

  to {
    transform: $rotate-skew translate(-$shadowfull, 0);
  }
}

@keyframes shadow-three {
  from {
    transform: $rotate-skew translate(0, $shadowfull);
  }

  50% {
    transform: $rotate-skew translate(0, $shadowfull);
  }

  to {
    transform: $rotate-skew translate(0, $shadowfull * 2);
  }
}

@keyframes shadow-four {
  from {
    transform: $rotate-skew translate(0, $shadowfull * 2);
  }

  50% {
    transform: $rotate-skew translate(-$shadowfull, $shadowfull * 2);
  }

  to {
    transform: $rotate-skew translate(-$shadowfull, $shadowfull);
  }
</style>
<div class="container">
  <div class="cube">
    <div class="top"></div>
    <div class="left"></div>
    <div class="right"></div>
  </div>
  <div class="cube">
    <div class="top"></div>
    <div class="left"></div>
    <div class="right"></div>
  </div>
  <div class="cube">
    <div class="top"></div>
    <div class="left"></div>
    <div class="right"></div>
  </div>
  <div class="cube">
    <div class="top"></div>
    <div class="left"></div>
    <div class="right"></div>
  </div>
  <div class="shadow">
    <div class="one"></div>
    <div class="two"></div>
    <div class="three"></div>
    <div class="four"></div>
  </div>
</div>
<H1> WELCOME TO KOIHATSU BY AYUSHMAN </H1>
<div class="navbar">
  <a href="#home">Home</a>
  <a href="#news">News</a>
  <div class="dropdown">
    <button class="dropbtn">More
      <i class="fa fa-caret-down"></i>
    </button>
    
</body>

    

