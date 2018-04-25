<template>
  <v-jumbotron :gradient="gradient" height="91.1vh" style="margin-top: 1px;">
    <v-flex text-xs-center>
      <v-layout align-center justify-center>
        <div class="css-typing">
          <p id="ml3">
            let developer: { <!-- p1 -->
          </p>
          <p id="ml5">
            name: 'Marcelo Nogueira da Silva', <!-- p2 -->
          </p>
          <p id="ml5">
            education: 'computer engineering', <!-- p3 -->
          </p>
          <p id="ml5">
            skills: [ <!-- p4 -->
          </p>
          <p id="ml7">
            'html', <!-- p5 -->
          </p>
          <p id="ml7">
            'css', <!-- p6 -->
          </p>
          <p id="ml7">
            'JavaScript', <!-- p7 -->
          </p>
          <p id="ml7">
            'NodeJS', <!-- p8 -->
          </p>
          <p id="ml7">
            'VueJS', <!-- p9 -->
          </p>
          <p id="ml7">
            'PHP', <!-- p10 -->
          </p>
          <p id="ml7">
            'Laravel'] <!-- p11 -->
          </p>
          <p id="ml3">
            } <!-- p12 -->
          </p>
        </div>
      </v-layout>
    </v-flex>
    <v-footer fixed>
      <v-spacer>
        <a href="https://github.com/locemarn" target="_blank" id="icon" ><v-icon dark>fab fa-github</v-icon></a>
        <a href="https://www.linkedin.com/in/marcelo-nogueira-408920109/" target="_blank" id="icon"><v-icon dark>fab fa-linkedin-in</v-icon></a>
        <a href="https://drive.google.com/open?id=1O_zG12-y2UPFIAAEuHynFd2Y5Zi7xYW2" target="_blank" id="icon"><v-icon dark>far fa-file-pdf</v-icon></a>
        <a href="https://locemarn.github.io/marceloNogueira/" target="_blank" id="icon" ><v-icon dark>fas fa-laptop</v-icon></a>
      </v-spacer>
    </v-footer>
  </v-jumbotron>
</template>

<script>
export default {
  data: () => ({
    gradient: 'to top, #CCE8CB, #FFF'
  })
}
</script>

<style>
#ml3 {
  margin-left: 2%;
}

#ml5 {
  margin-left: 5%;
}

#ml7 {
  margin-left: 10%;
}

#icon {
  padding: 2%;
  /* margin: 1%; */
  color: #008080;
}

#icon:hover {
  color: #012300;
}

.css-typing {
  margin-top: 5%;
}

.css-typing p {
  border-right: .15em solid #008080;
  font-family: "Courier";
  font-size: 16px;
  white-space: nowrap;
  overflow: hidden;
  color: #008080;
  margin: 0;
}

.css-typing p:nth-child(1) {
  width: 9.6em;
  -webkit-animation: type 2s steps(40, end);
  animation: type 2s steps(40, end);
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

.css-typing p:nth-child(2) {
  width: 20.5em;
  opacity: 0;
  -webkit-animation: type2 3s steps(40, end);
  animation: type2 3s steps(40, end);
  -webkit-animation-delay: 2s;
  animation-delay: 2s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

.css-typing p:nth-child(3) {
  width: 20.5em;
  opacity: 0;
  -webkit-animation: type3 3s steps(40, end);
  animation: type3 3s steps(40, end);
  -webkit-animation-delay: 5s;
  animation-delay: 5s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

.css-typing p:nth-child(4) {
  width: 5.5em;
  opacity: 0;
  -webkit-animation: type4 2s steps(40, end);
  animation: type4 2s steps(40, end);
  -webkit-animation-delay: 8s;
  animation-delay: 8s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

.css-typing p:nth-child(5) {
  width: 4.5em;
  opacity: 0;
  -webkit-animation: type5 1s steps(40, end);
  animation: type5 1s steps(40, end);
  -webkit-animation-delay: 10s;
  animation-delay: 10s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

.css-typing p:nth-child(6) {
  width: 3.5em;
  opacity: 0;
  -webkit-animation: type6 1s steps(40, end);
  animation: type6 1s steps(40, end);
  -webkit-animation-delay: 11s;
  animation-delay: 11s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

.css-typing p:nth-child(7) {
  width: 8em;
  opacity: 0;
  -webkit-animation: type6 2s steps(40, end);
  animation: type6 2s steps(40, end);
  -webkit-animation-delay: 12s;
  animation-delay: 12s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

.css-typing p:nth-child(8) {
  width: 6em;
  opacity: 0;
  -webkit-animation: type7 1s steps(40, end);
  animation: type7 1s steps(40, end);
  -webkit-animation-delay: 14s;
  animation-delay: 14s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

.css-typing p:nth-child(9) {
  width: 5em;
  opacity: 0;
  -webkit-animation: type7 1s steps(40, end);
  animation: type7 1s steps(40, end);
  -webkit-animation-delay: 15s;
  animation-delay: 15s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

.css-typing p:nth-child(10) {
  width: 4em;
  opacity: 0;
  -webkit-animation: type7 1s steps(40, end);
  animation: type7 1s steps(40, end);
  -webkit-animation-delay: 16s;
  animation-delay: 16s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

.css-typing p:nth-child(11) {
  width: 6em;
  opacity: 0;
  -webkit-animation: type7 2s steps(40, end);
  animation: type7 2s steps(40, end);
  -webkit-animation-delay: 17s;
  animation-delay: 17s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

/* .css-typing p:nth-child(12) {
  width: 2em;
  opacity: 0;
  -webkit-animation: type7 1s steps(40, end);
  animation: type7 1s steps(40, end);
  -webkit-animation-delay: 19s;
  animation-delay: 19s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
} */

.css-typing p:nth-child(12) {
  width: .7em;
  opacity: 0;
  -webkit-animation: type12 1s steps(20, end), blink .5s step-end infinite alternate;
  animation: type12 1s steps(20, end), blink .5s step-end infinite alternate;
  -webkit-animation-delay: 19s;
  animation-delay: 19s;
  -webkit-animation-fill-mode: forwards;
  animation-fill-mode: forwards;
}

@keyframes type {
  0% {
    width: 0;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    border: none;
  }
}

@-webkit-keyframes type {
  0% {
    width: 0;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    border: none;
  }
}

@keyframes type2 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@-webkit-keyframes type2 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@keyframes type3 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@-webkit-keyframes type3 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@keyframes type4 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@-webkit-keyframes type4 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@keyframes type5 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@-webkit-keyframes type5 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@keyframes type6 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@-webkit-keyframes type6 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@keyframes type7 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@-webkit-keyframes type7 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@keyframes type8 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@-webkit-keyframes type8 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@keyframes type9 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@-webkit-keyframes type9 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@keyframes type10 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@-webkit-keyframes type10 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@keyframes type11 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

@-webkit-keyframes type11 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
}

/* @keyframes type12 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #012300;
  }
  100% {
    opacity: 1;
    border: none;
  }
} */

/* @-webkit-keyframes type12 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  99.9% {
    border-right: .15em solid #008080;
  }
  100% {
    opacity: 1;
    border: none;
  }
} */

@keyframes type12 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  100% {
    opacity: 1;
  }
}

@-webkit-keyframes type12 {
  0% {
    width: 0;
  }
  1% {
    opacity: 1;
  }
  100% {
    opacity: 1;
  }
}

@keyframes blink {
  50% {
    border-color: transparent;
  }
}
@-webkit-keyframes blink {
  50% {
    border-color: tranparent;
  }
}
</style>
