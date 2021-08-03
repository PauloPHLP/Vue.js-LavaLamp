<template>
  <div class="lava-container">
    <div class="lava" />
    <div class="lava" />
    <div class="lava" />
    <div class="lava" />
    <div class="lava" />
    <div class="lava" />
    <div class="lava" />
    <div class="lava" />
    <div class="lava" />
    <div class="lava" />
    <div class="lava" />
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
  overflow: hidden;
}

.lava {
  background-color: #226b9b;
  border-radius: 50%;
  position: absolute;
}

.lava:nth-child(1) {
  width: 300px;
  height: 300px;
  position: absolute;
  left: 35%;
  top: 15%;
  animation: lava-one ease-in-out 32s infinite, deform 3s ease-in-out alternate infinite;
}

.lava:nth-child(2) {
  width: 400px;
  height: 400px;
  position: absolute;
  right: 24%;
  bottom: 65%;
  animation: lava-two ease-in-out 24s infinite, deform 4s ease-in-out alternate infinite;
}

.lava:nth-child(3) {
  width: 150px;
  height: 150px;
  bottom: -15%;
  left: 34%;
  animation: lava-three ease-in-out 32s infinite, deform 6s ease-in-out alternate infinite;
}

.lava:nth-child(4) {
  width: 235px;
  height: 235px;
  bottom: -19%;
  left: 30%;
  animation: lava-four ease-in-out 24s infinite, deform 2s ease-in-out alternate infinite;
}

.lava:nth-child(5) {
  width: 235px;
  height: 235px;
  bottom: -19%;
  left: 30%;
  animation: lava-five ease-in-out 32s infinite, deform 4s ease-in-out alternate infinite;
}

.lava:nth-child(6) {
  width: 55px;
  height: 55px;
  bottom: -25%;
  left: 34%;
  animation: lava-six ease-in-out 24s infinite, deform 6s ease-in-out alternate infinite;
}

.lava:nth-child(7) {
  width: 35px;
  height: 35px;
  bottom: -25%;
  right: 34%;
  animation: lava-seven ease-in-out 32s infinite, deform 4s ease-in-out alternate infinite;
}

.lava:nth-child(8) {
  width: 435px;
  height: 435px;
  bottom: -85%;
  right: 40%;
  animation: lava-eight ease-in-out 24s infinite, deform 6s ease-in-out alternate infinite;
}

.lava:nth-child(9) {
  width: 235px;
  height: 235px;
  bottom: -15%;
  right: 10%;
  animation: lava-nine ease-in-out 32s infinite, deform 2s ease-in-out alternate infinite;
}

.lava:nth-child(10) {
  width: 135px;
  height: 135px;
  bottom: 12%;
  right: 10%;
  animation: lava-ten ease-in-out 24s infinite, deform 4s ease-in-out alternate infinite;
}

.lava:nth-child(11) {
  width: 500px;
  height: 500px;
  bottom: 0%;
  left: 0%;
  animation: lava-eleven ease-in-out 32s infinite, deform 2s ease-in-out alternate infinite;
}

.lava:nth-child(12) {
  width: 335px;
  height: 335px;
  bottom: 20%;
  left: 20%;
  animation: lava-twelve ease-in-out 24s infinite, deform 4s ease-in-out alternate infinite;
}

@keyframes deform {
  50% {
    border-radius: 40% 60% 70% 30% / 45% 45% 55% 55%;
  }
  100% {
    border-radius: 30% 50% 75% 36% / 50% 40% 50% 60%;
  }
}

@keyframes spin {
  /* from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(360deg);
  } */
}

@keyframes scale {
  /* 0% {
    transform: scale(100%);
  }

  100% {
    transform: scale(150%);
  } */
}

@keyframes lava-one {
  0%,
  100% {
    transform: translatey(0);
  }
  50% {
    transform: translatey(700%);
  }
}

@keyframes lava-two {
  0%,
  100% {
    transform: translatey(0);
  }
  50% {
    transform: translatey(420%);
  }
}

@keyframes lava-three {
  0%,
  100% {
    transform: translatey(0);
  }
  50% {
    transform: translatey(-305%);
  }
}

@keyframes lava-four {
  0%,
  100% {
    transform: translatey(0);
  }
  50% {
    transform: translatey(-605%);
  }
}

@keyframes lava-five {
  0%,
  100% {
    transform: translatey(0);
  }
  50% {
    transform: translatey(-700%);
  }
}

@keyframes lava-six {
  0%,
  100% {
    transform: translatey(0);
  }
  50% {
    transform: translatey(-700%);
  }
}

@keyframes lava-seven {
  0%,
  100% {
    transform: translatey(0);
  }
  50% {
    transform: translatey(-300%);
  }
}

@keyframes lava-eight {
  0%,
  100% {
    transform: translatey(0);
  }
  50% {
    transform: translatey(-700%);
  }
}

@keyframes lava-nine {
  0%,
  100% {
    transform: translatey(0);
  }
  50% {
    transform: translatey(200%);
  }
}

@keyframes lava-ten {
  0%,
  100% {
    transform: translatey(0);
  }
  50% {
    transform: translatey(-700%);
  }
}

@keyframes lava-eleven {
  0%,
  100% {
    transform: translatey(0);
  }
  50% {
    transform: translatey(200%);
  }
}

@keyframes lava-twelve {
  0%,
  100% {
    transform: translatey(0);
  }
  50% {
    transform: translatey(-300%);
  }
}
</style>
