<template>
  <div class="lava-container">
    <!-- Group 1 -->
    <div class="lava-element lava" />
    <div class="lava-element square" />
    <div class="lava-element triangle" />
    <div class="lava-element square" />
    <div class="lava-element lava" />
    <div class="lava-element square" />
    <div class="lava-element square" />
    <div class="lava-element triangle" />
    <div class="lava-element square" />
    <div class="lava-element lava" />
    <div class="lava-element triangle" />
    <div class="lava-element square" />

    <!-- Group 2 -->
    <div class="lava-element square" />
    <div class="lava-element lava" />
    <div class="lava-element triangle" />
    <div class="lava-element square" />
    <div class="lava-element triangle" />
    <div class="lava-element square" />
    <div class="lava-element square" />
    <div class="lava-element triangle" />
    <div class="lava-element square" />
    <div class="lava-element square" />
    <div class="lava-element lava" />
    <div class="lava-element triangle" />

    <!-- Group 3 -->
    <div class="lava-element lava" />
    <div class="lava-element square" />
    <div class="lava-element lava" />
    <div class="lava-element triangle" />
    <div class="lava-element square" />
    <div class="lava-element triangle" />
    <div class="lava-element lava" />
    <div class="lava-element square" />
    <div class="lava-element square" />
    <div class="lava-element triangle" />
    <div class="lava-element square" />
    <div class="lava-element square" />

    <!-- Group 4 -->
    <div class="lava-element lava" />
    <div class="lava-element triangle" />
    <div class="lava-element lava" />
    <div class="lava-element square" />
    <div class="lava-element lava" />
    <div class="lava-element lava" />
    <div class="lava-element square" />
    <div class="lava-element lava" />
    <div class="lava-element triangle" />
    <div class="lava-element lava" />
    <div class="lava-element square" />
    <div class="lava-element lava" />

    <!-- Group 5 -->
    <div class="lava-element lava" />
    <div class="lava-element square" />
    <div class="lava-element lava" />
    <div class="lava-element triangle" />
    <div class="lava-element lava" />
    <div class="lava-element triangle" />
    <div class="lava-element triangle" />
    <div class="lava-element lava" />
    <div class="lava-element lava" />
    <div class="lava-element square" />
    <div class="lava-element square" />
    <div class="lava-element lava" />

    <!-- Group 6 -->
    <div class="lava-element lava" />
    <div class="lava-element square" />
    <div class="lava-element square" />
    <div class="lava-element lava" />
    <div class="lava-element lava" />
    <div class="lava-element triangle" />
    <div class="lava-element triangle" />
    <div class="lava-element lava" />
    <div class="lava-element triangle" />
    <div class="lava-element lava" />
    <div class="lava-element square" />
    <div class="lava-element lava" />
  </div>
</template>

<script>
export default {
  name: 'LavaLamp'
}
</script>

<style lang="scss" scoped>
/* Container style */
.lava-container {
  background-color: #1b6798;
  height: 100vh;
  width: inherit;
  display: flex;
  align-items: center;
  justify-content: center;
  position: absolute;
  top: 0;
  left: 0;
  overflow: hidden;
  z-index: -1;

  & * {
    box-shadow: rgba(99, 99, 99, 0.2) 0px 8px 24px;
  }
}

/* Default styles for each element type */

.lava-element.lava {
  background-color: #226b9b;
  border-radius: 50%;
  position: absolute;
}

.lava-element.square {
  position: absolute;
  background: #226b9b;
}

.lava-element.triangle {
  width: 0;
  height: 0;
  position: absolute;
}

/* Lava elements styles */

/* Group 1 */

.lava-element:nth-child(1) {
  width: 200px;
  height: 200px;
  left: 35%;
  top: 15%;
  opacity: 0.4;
  animation: animation-one ease-in-out 54s infinite;
}

.lava-element:nth-child(2) {
  width: 180px;
  height: 180px;
  right: 50%;
  bottom: 55%;
  opacity: 0.75;
  animation: animation-two ease-in-out 48s infinite;
}

.lava-element:nth-child(3) {
  border-top: 17px solid #226b9b;
  border-left: 17px solid transparent;
  bottom: 0%;
  left: 0%;
  opacity: 0.3;
  animation: animation-seven ease-in-out 54s infinite;
}

.lava-element:nth-child(4) {
  border-top: 10px solid #226b9b;
  border-right: 10px solid transparent;
  bottom: -19%;
  left: 30%;
  opacity: 1;
  animation: animation-four ease-in-out 48s infinite;
}

.lava-element:nth-child(5) {
  width: 12px;
  height: 12px;
  bottom: -19%;
  left: 45%;
  opacity: 1;
  animation: animation-five ease-in-out 54s infinite;
}

.lava-element:nth-child(6) {
  width: 5px;
  height: 5px;
  bottom: -25%;
  left: 20%;
  opacity: 0.75;
  animation: animation-six ease-in-out 48s infinite;
}

.lava-element:nth-child(7) {
  width: 35px;
  height: 35px;
  bottom: 25%;
  right: 34%;
  opacity: 0.4;
  animation: animation-seven ease-in-out 54s infinite;
}

.lava-element:nth-child(8) {
  border-bottom: 210px solid #226b9b;
  border-left: 210px solid transparent;
  bottom: -85%;
  right: 40%;
  opacity: 0.3;
  animation: animation-eight ease-in-out 48s infinite;
}

.lava-element:nth-child(9) {
  width: 235px;
  height: 235px;
  bottom: -5%;
  right: 10%;
  opacity: 0.75;
  animation: animation-nine ease-in-out 54s infinite;
}

.lava-element:nth-child(10) {
  width: 135px;
  height: 135px;
  bottom: 20%;
  right: 15%;
  opacity: 1;
  animation: animation-ten ease-in-out 48s infinite;
}

.lava-element:nth-child(11) {
  border-top: 17px solid #226b9b;
  border-left: 17px solid transparent;
  bottom: 0%;
  left: 0%;
  opacity: 0.75;
  animation: animation-eleven ease-in-out 54s infinite;
}

.lava-element:nth-child(12) {
  width: 155px;
  height: 155px;
  bottom: 30%;
  left: 22%;
  opacity: 0.4;
  animation: animation-twelve ease-in-out 48s infinite;
}

/* Group 2 */

.lava-element:nth-child(13) {
  width: 20px;
  height: 20px;
  left: 35%;
  top: 15%;
  opacity: 0.3;
  animation: animation-two ease-in-out 54s infinite;
}

.lava-element:nth-child(14) {
  width: 8px;
  height: 8px;
  right: 50%;
  bottom: 55%;
  opacity: 1;
  animation: animation-four ease-in-out 48s infinite;
}

.lava-element:nth-child(15) {
  border-bottom: 10px solid #226b9b;
  border-left: 10px solid transparent;
  bottom: -85%;
  right: 40%;
  opacity: 0.3;
  animation: animation-nine ease-in-out 48s infinite;
}

.lava-element:nth-child(16) {
  width: 35px;
  height: 35px;
  bottom: 12%;
  right: 15%;
  opacity: 0.2;
  animation: animation-three ease-in-out 48s infinite;
}

.lava-element:nth-child(17) {
  border-top: 10px solid #226b9b;
  border-left: 10px solid transparent;
  bottom: 0%;
  left: 0%;
  opacity: 0.4;
  animation: animation-eleven ease-in-out 54s infinite;
}

.lava-element:nth-child(18) {
  width: 55px;
  height: 55px;
  bottom: 20%;
  left: 10%;
  opacity: 0.75;
  animation: animation-five ease-in-out 48s infinite;
}

.lava-element:nth-child(19) {
  width: 5px;
  height: 5px;
  bottom: -25%;
  left: 20%;
  opacity: 0.3;
  animation: animation-six ease-in-out 48s infinite;
}

.lava-element:nth-child(20) {
  border-bottom: 20px solid #226b9b;
  border-left: 20px solid transparent;
  bottom: -55%;
  right: 20%;
  opacity: 0.75;
  animation: animation-nine ease-in-out 48s infinite;
}

.lava-element:nth-child(21) {
  width: 50px;
  height: 50px;
  bottom: -15%;
  left: 50%;
  opacity: 0.4;
  animation: animation-one ease-in-out 54s infinite;
}

.lava-element:nth-child(22) {
  width: 23px;
  height: 23px;
  bottom: 12%;
  right: 45%;
  opacity: 0.75;
  animation: animation-seven ease-in-out 54s infinite;
}

.lava-element:nth-child(23) {
  width: 13px;
  height: 13px;
  bottom: 30%;
  right: 70%;
  opacity: 1;
  animation: animation-twelve ease-in-out 48s infinite;
}

.lava-element:nth-child(24) {
  border-top: 15px solid #226b9b;
  border-left: 15px solid transparent;
  bottom: 5%;
  left: 10%;
  opacity: 1;
  animation: animation-twelve ease-in-out 54s infinite;
}

/* Group 3 */

.lava-element:nth-child(25) {
  width: 10px;
  height: 10px;
  bottom: 35%;
  right: 20%;
  opacity: 0.2;
  animation: animation-seven ease-in-out 54s infinite;
}

.lava-element:nth-child(26) {
  width: 25px;
  height: 25px;
  bottom: 25%;
  right: 34%;
  opacity: 0.4;
  animation: animation-eight ease-in-out 54s infinite;
}

.lava-element:nth-child(27) {
  width: 12px;
  height: 12px;
  bottom: -15%;
  right: 20%;
  opacity: 0.4;
  animation: animation-ten ease-in-out 54s infinite;
}

.lava-element:nth-child(28) {
  border-top: 15px solid #226b9b;
  border-left: 15px solid transparent;
  bottom: -12%;
  left: 5%;
  opacity: 0.3;
  animation: animation-two ease-in-out 54s infinite;
}

.lava-element:nth-child(29) {
  width: 13px;
  height: 13px;
  bottom: 15%;
  right: 12%;
  opacity: 0.2;
  animation: animation-eleven ease-in-out 48s infinite;
}

.lava-element:nth-child(30) {
  border-bottom: 10px solid #226b9b;
  border-left: 10px solid transparent;
  bottom: -15%;
  right: 85%;
  opacity: 0.75;
  animation: animation-seven ease-in-out 48s infinite;
}

.lava-element:nth-child(31) {
  width: 20px;
  height: 20px;
  bottom: 15%;
  left: 10%;
  opacity: 0.3;
  animation: animation-one ease-in-out 48s infinite;
}

.lava-element:nth-child(32) {
  width: 5px;
  height: 5px;
  bottom: -20%;
  left: 25%;
  opacity: 0.75;
  animation: animation-three ease-in-out 48s infinite;
}

.lava-element:nth-child(33) {
  width: 13px;
  height: 13px;
  top: 15%;
  right: 12%;
  opacity: 0.4;
  animation: animation-eight ease-in-out 48s infinite;
}

.lava-element:nth-child(34) {
  border-bottom: 120px solid #226b9b;
  border-left: 120px solid transparent;
  bottom: -40%;
  right: 85%;
  opacity: 0.3;
  animation: animation-eight ease-in-out 48s infinite;
}

.lava-element:nth-child(35) {
  width: 11px;
  height: 11px;
  bottom: 34%;
  right: 60%;
  opacity: 0.4;
  animation: animation-five ease-in-out 54s infinite;
}

.lava-element:nth-child(36) {
  width: 15px;
  height: 15px;
  bottom: -15%;
  left: 50%;
  opacity: 0.3;
  animation: animation-three ease-in-out 54s infinite;
}

/* Group 4 */

.lava-element:nth-child(37) {
  width: 12px;
  height: 12px;
  bottom: -20%;
  left: 25%;
  opacity: 0.4;
  animation: animation-six ease-in-out 48s infinite;
}

.lava-element:nth-child(38) {
  border-bottom: 270px solid #226b9b;
  border-left: 270px solid transparent;
  top: -5%;
  right: 15%;
  opacity: 0.4;
  animation: animation-seven ease-in-out 48s infinite;
}

.lava-element:nth-child(39) {
  width: 50px;
  height: 50px;
  bottom: -20%;
  left: 25%;
  opacity: 0.3;
  animation: animation-eight ease-in-out 48s infinite;
}

.lava-element:nth-child(40) {
  border-top: 112px solid #226b9b;
  border-left: 112px solid transparent;
  bottom: -5%;
  left: 12%;
  opacity: 0.2;
  animation: animation-two ease-in-out 54s infinite;
}

.lava-element:nth-child(41) {
  width: 115px;
  height: 115px;
  bottom: 25%;
  right: 34%;
  opacity: 0.75;
  animation: animation-five ease-in-out 54s infinite;
}

.lava-element:nth-child(42) {
  width: 17px;
  height: 17px;
  bottom: 34%;
  right: 25%;
  opacity: 1;
  animation: animation-one ease-in-out 54s infinite;
}

.lava-element:nth-child(43) {
  width: 25px;
  height: 25px;
  bottom: 15%;
  right: 20%;
  opacity: 1;
  animation: animation-eight ease-in-out 54s infinite;
}

.lava-element:nth-child(44) {
  border-bottom: 7px solid #226b9b;
  border-left: 7px solid transparent;
  bottom: -40%;
  right: 20%;
  opacity: 0.75;
  animation: animation-nine ease-in-out 48s infinite;
}

.lava-element:nth-child(45) {
  border-top: 8px solid #226b9b;
  border-left: 8px solid transparent;
  bottom: 10%;
  left: 19%;
  opacity: 0.4;
}

.lava-element:nth-child(46) {
  width: 12px;
  height: 12px;
  bottom: -45%;
  left: 19%;
  opacity: 0.3;
  animation: animation-three ease-in-out 54s infinite;
}

.lava-element:nth-child(47) {
  width: 5px;
  height: 5px;
  bottom: -10%;
  left: 18%;
  opacity: 0.75;
  animation: animation-four ease-in-out 48s infinite;
}

.lava-element:nth-child(48) {
  width: 45px;
  height: 45px;
  bottom: 34%;
  right: 22%;
  opacity: 0.75;
  animation: animation-seven ease-in-out 54s infinite;
}

/* Group 5 */

.lava-element:nth-child(49) {
  width: 10px;
  height: 23px;
  bottom: -8%;
  right: 12%;
  opacity: 0.75;
  animation: animation-ten ease-in-out 54s infinite;
}

.lava-element:nth-child(50) {
  width: 13px;
  height: 13px;
  bottom: 50%;
  right: 10%;
  opacity: 1;
  animation: animation-two ease-in-out 48s infinite;
}

.lava-element:nth-child(51) {
  width: 13px;
  height: 13px;
  bottom: -10%;
  right: 5%;
  opacity: 0.4;
  animation: animation-ten ease-in-out 54s infinite;
}

.lava-element:nth-child(52) {
  border-bottom: 7px solid #226b9b;
  border-left: 7px solid transparent;
  bottom: -32%;
  right: 15%;
  opacity: 0.75;
  animation: animation-nine ease-in-out 48s infinite;
}

.lava-element:nth-child(53) {
  width: 6px;
  height: 6px;
  bottom: -5%;
  right: 10%;
  opacity: 0.4;
  animation: animation-ten ease-in-out 54s infinite;
}

.lava-element:nth-child(54) {
  border-top: 5px solid #226b9b;
  border-left: 5px solid transparent;
  bottom: 15%;
  left: 15%;
  opacity: 0.4;
  animation: animation-eleven ease-in-out 54s infinite;
}

.lava-element:nth-child(55) {
  border-top: 4px solid #226b9b;
  border-right: 4px solid transparent;
  bottom: -1%;
  left: 19%;
  opacity: 1;
  animation: animation-four ease-in-out 48s infinite;
}

.lava-element:nth-child(56) {
  width: 10px;
  height: 10px;
  top: 15%;
  left: 12%;
  opacity: 1;
  animation: animation-seven ease-in-out 48s infinite;
}

.lava-element:nth-child(57) {
  width: 2px;
  height: 2px;
  bottom: -19%;
  left: 45%;
  opacity: 0.3;
  animation: animation-three ease-in-out 54s infinite;
}

.lava-element:nth-child(58) {
  width: 6px;
  height: 6px;
  bottom: -4%;
  left: 25%;
  opacity: 0.3;
  animation: animation-three ease-in-out 54s infinite;
}

.lava-element:nth-child(59) {
  width: 8px;
  height: 8px;
  bottom: -10%;
  right: 5%;
  opacity: 0.75;
  animation: animation-ten ease-in-out 54s infinite;
}

.lava-element:nth-child(60) {
  width: 12px;
  height: 12px;
  bottom: -19%;
  left: 45%;
  opacity: 1;
  animation: animation-five ease-in-out 54s infinite;
}

/* Group 6 */

.lava-element:nth-child(61) {
  width: 12px;
  height: 12px;
  top: 19%;
  right: 45%;
  opacity: 1;
  animation: animation-five ease-in-out 54s infinite;
}

.lava-element:nth-child(62) {
  width: 8px;
  height: 8px;
  top: 10%;
  left: 5%;
  opacity: 0.75;
  animation: animation-ten ease-in-out 54s infinite;
}

.lava-element:nth-child(63) {
  width: 6px;
  height: 6px;
  top: 4%;
  right: 25%;
  opacity: 0.3;
  animation: animation-three ease-in-out 54s infinite;
}

.lava-element:nth-child(64) {
  width: 2px;
  height: 2px;
  top: 19%;
  right: 45%;
  opacity: 0.3;
  animation: animation-three ease-in-out 54s infinite;
}

.lava-element:nth-child(65) {
  width: 10px;
  height: 10px;
  bottom: 15%;
  right: 12%;
  opacity: 1;
  animation: animation-seven ease-in-out 48s infinite;
}

.lava-element:nth-child(66) {
  border-top: 4px solid #226b9b;
  border-right: 4px solid transparent;
  top: 1%;
  right: 19%;
  opacity: 1;
  animation: animation-four ease-in-out 48s infinite;
}

.lava-element:nth-child(67) {
  border-top: 20px solid #226b9b;
  border-left: 110px solid transparent;
  top: 15%;
  right: 15%;
  opacity: 0.4;
  animation: animation-eleven ease-in-out 54s infinite;
}

.lava-element:nth-child(68) {
  width: 6px;
  height: 6px;
  top: 5%;
  left: 10%;
  opacity: 0.4;
  animation: animation-ten ease-in-out 54s infinite;
}

.lava-element:nth-child(69) {
  border-bottom: 7px solid #226b9b;
  border-left: 7px solid transparent;
  top: 32%;
  left: 15%;
  opacity: 0.75;
  animation: animation-nine ease-in-out 48s infinite;
}

.lava-element:nth-child(70) {
  width: 13px;
  height: 13px;
  top: 10%;
  left: 5%;
  opacity: 0.4;
  animation: animation-ten ease-in-out 54s infinite;
}

.lava-element:nth-child(71) {
  width: 13px;
  height: 13px;
  top: 50%;
  right: 70%;
  opacity: 1;
  animation: animation-two ease-in-out 48s infinite;
}

.lava-element:nth-child(72) {
  width: 10px;
  height: 23px;
  top: 8%;
  right: 12%;
  opacity: 0.75;
  animation: animation-ten ease-in-out 54s infinite;
}

/* Animations */

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
