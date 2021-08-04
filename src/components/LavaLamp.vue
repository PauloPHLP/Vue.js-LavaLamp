<template>
  <div class="lava-container">
    <div class="lava" />
    <div class="square" />
    <div class="lava" />
    <div class="triangle" />
    <div class="lava" />
    <div class="square" />
    <div class="lava" />
    <div class="triangle" />
    <div class="square" />
    <div class="lava" />
    <div class="triangle" />
    <div class="lava" />
  </div>
</template>

<script>
export default {
  name: 'LavaLamp'
}
</script>

<style lang="scss" scoped>
.lava-container {
  background-color: #1b6798;
  height: 100vh;
  width: 100vw;
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  overflow: hidden;
}

.lava {
  background-color: #226b9b;
  border-radius: 50%;
  position: absolute;
}

.lava:nth-child(1) {
  width: 200px;
  height: 200px;
  left: 35%;
  top: 15%;
  animation: animation-one ease-in-out 54s infinite, deform 2s ease-in-out alternate infinite;
}

.square:nth-child(2) {
  width: 200px;
  height: 200px;
  position: absolute;
  right: 24%;
  bottom: 65%;
  background: #226b9b;
  animation: animation-two ease-in-out 48s infinite;
}

.lava:nth-child(3) {
  width: 150px;
  height: 150px;
  bottom: -15%;
  left: 50%;
  animation: animation-three ease-in-out 54s infinite, deform 2s ease-in-out alternate infinite;
}

.triangle:nth-child(4) {
  width: 0;
  height: 0;
  border-top: 130px solid #226b9b;
  border-right: 270px solid transparent;
  position: absolute;
  bottom: -19%;
  left: 30%;
  animation: animation-four ease-in-out 48s infinite;
}

.lava:nth-child(5) {
  width: 125px;
  height: 125px;
  bottom: -19%;
  left: 45%;
  animation: animation-five ease-in-out 54s infinite, deform 2s ease-in-out alternate infinite;
}

.square:nth-child(6) {
  width: 55px;
  height: 55px;
  position: absolute;
  bottom: -25%;
  left: 20%;
  background: #226b9b;
  animation: animation-six ease-in-out 48s infinite;
}

.lava:nth-child(7) {
  width: 35px;
  height: 35px;
  bottom: 25%;
  right: 34%;
  animation: animation-seven ease-in-out 54s infinite, deform 2s ease-in-out alternate infinite;
}

.triangle:nth-child(8) {
  width: 0;
  height: 0;
  border-bottom: 200px solid #226b9b;
  border-left: 200px solid transparent;
  position: absolute;
  bottom: -85%;
  right: 40%;
  animation: animation-eight ease-in-out 48s infinite;
}

.square:nth-child(9) {
  width: 235px;
  height: 235px;
  position: absolute;
  bottom: -5%;
  right: 10%;
  background: #226b9b;
  animation: animation-nine ease-in-out 54s infinite;
}

.lava:nth-child(10) {
  width: 135px;
  height: 135px;
  bottom: 12%;
  right: 15%;
  animation: animation-ten ease-in-out 48s infinite, deform 4s ease-in-out alternate infinite;
}

.triangle:nth-child(11) {
  width: 0;
  height: 0;
  border-top: 170px solid #226b9b;
  border-left: 170px solid transparent;
  position: absolute;
  bottom: 0%;
  left: 0%;
  animation: animation-eleven ease-in-out 54s infinite;
}

.lava:nth-child(12) {
  width: 135px;
  height: 135px;
  bottom: 20%;
  left: 20%;
  animation: animation-twelve ease-in-out 48s infinite, deform 4s ease-in-out alternate infinite;
}

@keyframes deform {
  50% {
    border-radius: 40% 60% 70% 30% / 45% 45% 55% 55%;
  }
  100% {
    border-radius: 30% 50% 75% 36% / 50% 40% 50% 60%;
  }
}

@keyframes animation-one {
  0% {
    transform: translatey(0) scale(100%) rotate(0deg);
  }
  50% {
    transform: translatey(700%) scale(150%) rotate(180deg);
  }
  100% {
    transform: translatey(0) scale(100%) rotate(360deg);
  }
}

@keyframes animation-two {
  0% {
    transform: translatey(0) scale(100%) rotate(0deg);
  }
  50% {
    transform: translatey(420%) scale(70%) rotate(180deg);
  }
  100% {
    transform: translatey(0) scale(100%) rotate(360deg);
  }
}

@keyframes animation-three {
  0% {
    transform: translatey(0) scale(100%) rotate(0deg);
  }
  25% {
    transform: translatey(-150%) scale(150%) rotate(90deg);
  }
  50% {
    transform: translatey(-300%) scale(80%) rotate(180deg);
  }
  100% {
    transform: translatey(0) scale(100%) rotate(360deg);
  }
}

@keyframes animation-four {
  0% {
    transform: translatey(0) scale(100%) rotate(0deg);
  }
  50% {
    transform: translatey(-605%) scale(130%) rotate(180deg);
  }
  100% {
    transform: translatey(0) scale(100%) rotate(360deg);
  }
}

@keyframes animation-five {
  0% {
    transform: translatey(0) scale(100%) rotate(0deg);
  }
  25% {
    transform: translatey(-350%) scale(70%) rotate(90deg);
  }
  50% {
    transform: translatey(-700%) scale(150%) rotate(180deg);
  }
  100% {
    transform: translatey(0) scale(100%) rotate(360deg);
  }
}

@keyframes animation-six {
  0% {
    transform: translatey(0) scale(100%) rotate(0deg);
  }
  50% {
    transform: translatey(-700%) scale(180%) rotate(180deg);
  }
  100% {
    transform: translatey(0) scale(100%) rotate(360deg);
  }
}

@keyframes animation-seven {
  0% {
    transform: translatey(0) scale(100%) rotate(0deg);
  }
  50% {
    transform: translatey(-700%) scale(150%) rotate(180deg);
  }
  100% {
    transform: translatey(0) scale(100%) rotate(360deg);
  }
}

@keyframes animation-eight {
  0% {
    transform: translatey(0) scale(100%) rotate(0deg);
  }
  50% {
    transform: translatey(-700%) scale(90%) rotate(180deg);
  }
  100% {
    transform: translatey(0) scale(100%) rotate(360deg);
  }
}

@keyframes animation-nine {
  0% {
    transform: translatey(0) scale(100%) rotate(0deg);
  }
  50% {
    transform: translatey(400%) scale(120%) rotate(180deg);
  }
  100% {
    transform: translatey(0) scale(100%) rotate(360deg);
  }
}

@keyframes animation-ten {
  0% {
    transform: translatey(0) scale(100%) rotate(0deg);
  }
  25% {
    transform: translatey(-350%) scale(140%) rotate(90deg);
  }
  50% {
    transform: translatey(-700%) scale(90%) rotate(180deg);
  }
  100% {
    transform: translatey(0) scale(100%) rotate(360deg);
  }
}

@keyframes animation-eleven {
  0% {
    transform: translatey(0) scale(100%) rotate(0deg);
  }
  50% {
    transform: translatey(200%) scale(110%) rotate(180deg);
  }
  100% {
    transform: translatey(0) scale(100%) rotate(360deg);
  }
}

@keyframes animation-twelve {
  0% {
    transform: translatey(0) scale(100%) rotate(0deg);
  }
  50% {
    transform: translatey(-300%) scale(170%) rotate(180deg);
  }
  100% {
    transform: translatey(0) scale(100%) rotate(360deg);
  }
}
</style>
