<template>
  <div class="container main">
    <div class="home tag">
      <span>Home</span>
    </div>
    <div class="animation">
      <svg id="レイヤー_1" data-name="レイヤー 1" class="abc" :class="className" xmlns="http://www.w3.org/2000/svg" >
        <polyline class="cls-1 svg-elem-1" points="389.54 352.5 411.02 352.5 1367 352.5"></polyline>
        <g class="cls-2">
          <line class="cls-3 svg-elem-2" x1="-1266" y1="257.5" x2="0.5" y2="257.5"></line>
        </g>
        <polygon class="cls-4 svg-elem-3" points="388.54 350.5 288.92 563.18 284.24 573.18 293.59 599 293.61 598.99 298.28 589.02 410.02 350.5 388.54 350.5"></polygon>
        <polygon class="cls-4 svg-elem-4" points="298.31 589.35 288.93 564.36 155.15 207.94 150.19 206.86 148.34 211.99 151.07 219.25 284.24 574.03 293.61 599 293.63 598.99 298.31 589.35"></polygon>
        <polygon class="cls-4 svg-elem-5" points="154.67 207.92 150.88 219 106 350.07 104.48 354.52 99.51 354.52 101.74 348 148.34 211.89 150.06 206.86 154.67 207.92"></polygon>
        <polygon class="cls-4 svg-elem-6" points="104.48 354.52 99.51 354.52 0.18 354.52 0.18 348 101.74 348 106 348 106 350.07 104.48 354.52"></polygon>
        <text class="cls-5" transform="translate(511.73 343.94)">Member</text>
      </svg>
    </div>
    <div class="container1">
      <div class="container-i-1">
        <img src="/member-yusei.jpg" height="" width="100%">
        <pre>
        <br>代表/豊永雄正
        </pre>
      </div>
      <div class="container-t-1">
        <h2>心が”ゆれる”ものを創る</h2>
        <br>
        <p>
          2020年9月16日、チームInovange『（イノベンジ）』を結成致しました。現在、メンバーは5人。僕自身の信念でもある”心がゆれるものを創る”を1つの理念として掲げております。<br><br>僕にとって、”ゆれる”は”つながる”であり、”革新”の意味。幼い頃から地元の福井で経験してきた人と”つながる”感覚。そして、TVや本、音楽を通して見続け、憧れ続けてきた”革新”。それらを表現していきます。まずは、広告やwebページを通してお客様とそのお客様を”つないで”いきます。
        </p>
      </div>
    </div>
    <div class="container2">
      <div class="container-i-2">
        <img src="/member-hiroto.jpg" height="" width="100%">
        <pre>
          <br>creater/加藤海澄
        </pre>
      </div>
      <div class="container-t-2">
        <h3>No laugh’n Nolife</h3>
        <br>
        <p>
          人が面白いと感じる瞬間はいつだと思いますか？お笑いに例えてみます。僕が1番の芸人として慕っているのが松本人志なのですが彼はトーク力が高いんです。後輩芸人に強気のツッコミ。年齢に負けないハイテクなボケ。そうきたか！その手があったか！と思わせるような奇想天外なトーク。僕はそれが面白いと感じる瞬間だと思います。お客様をアッと驚かせるような面白い広告、webを作ります。
        </p>
      </div>
    </div>
    <div class="container3">
      <div class="container-i-3">
        <img src="/member-yusei.jpg" height="" width="100%">
        <pre>
          <br>プログラマー/西沢至恩
        </pre>
      </div>
      <div class="container-t-3">
        <h3>三本柱</h3>
        <br>
        <p>
          ”普通”という言葉が嫌いです。服や持ち物が人とかぶるのが嫌いです。流行に乗りたくないです。人とかぶらない、”普通”じゃない革新的な広告、webデザインを任せてください！！
        </p>
      </div>
    </div>
    <div class="container4">
      <div class="container-i-4">
        <img src="/member-hiroto.jpg" height="" width="100%">
        <pre>
          <br>イラストレーター /照屋花音
        </pre>
      </div>
      <div class="container-t-4">
        <h4></h4>
        <br>
        <p></p>
      </div>
    </div>
    <div class="container5">
      <div class="container-i-5">
        <img src="/member-hiroto.jpg" height="" width="100%">
        <pre>
          <br>イラストレーター/深山れいか
        </pre>
      </div>
      <div class="container-t-5">
        <h4></h4>
        <br>
        <p></p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      active: false
    }
  },
  computed: {
    className () {
      return {
        active: this.active
      }
    }
  },
  mounted () {
    setTimeout(() => {
      this.active = true
    }, 50)
  }
}
</script>

<style>
.cls-1 {
  fill: #9a0010;
}

.cls-1, .cls-2, .cls-3 {
  stroke: #9a0010;
  stroke-miterlimit: 10;
}

.cls-1, .cls-2 {
  stroke-width: 1.51px;
}

.cls-2 {
  fill: #040000;
}

.cls-3 {
  fill: none;
  stroke-width: 2.24px;
}

.cls-4 {
  font-size: 66.4px;
  fill: #231815;
  font-family: KozGoPr6N-Regular-83pv-RKSJ-H, Kozuka Gothic Pr6N;
  letter-spacing: 0.18em;
}
span {
  border: 1px solid;
  border-color: #35495e;
}

.container-i-1 {
  width: 40%;
  float: left;
}

.container-t-1 {
  width: 50%;
  float: left;
  margin-left: 30px;
}

.container1 {
  margin: auto;
  margin-bottom: 140px;
  border: 2px solid black;
  width: 100%;
  height: 400px;
}

.container-i-2 {
  width: 40%;
  float: left;
}

.container-t-2 {
  width: 50%;
  float: left;
  margin-left: 30px;
}

.container2 {
  margin: auto;
  margin-bottom: 140px;
  border: 2px solid black;
  width: 100%;
  height: 400px;
}

.container-i-3 {
  width: 40%;
  float: left;
}

.container-t-3 {
  width: 50%;
  float: left;
  margin-left: 30px;
}

.container3 {
  margin: auto;
  margin-bottom: 140px;
  border: 2px solid black;
  width: 100%;
  height: 400px;
}

.container-i-4 {
  width: 40%;
  float: left;
}

.container-t-4 {
  width: 50%;
  float: left;
  margin-left: 30px;
}

.container4 {
  margin: auto;
  margin-bottom: 140px;
  border: 2px solid black;
  width: 100%;
  height: 400px;
}

.container-i-5 {
  width: 40%;
  float: left;
}

.container-t-5 {
  width: 50%;
  float: left;
  margin-left: 30px;
}

.container5 {
  margin: auto;
  margin-bottom: 140px;
  width: 100%;
  height: 400px;
}

.abc {
  width: 100%;
  height: 700px;
  position: absolute;
  top: 50%;
  left: 45%;
  transform: translate(-50%, -50%);
}

.animation {
  width: 1200px;
  height: 700px;
  position: relative;
}

@-webkit-keyframes animate-svg-stroke-1 {
  0% {
    stroke-dashoffset: 673.2532348632812px;
    stroke-dasharray: 673.2532348632812px;
  }

  100% {
    stroke-dashoffset: 0;
  }
}

@keyframes animate-svg-stroke-1 {
  0% {
    stroke-dashoffset: 673.2532348632812px;
    stroke-dasharray: 673.2532348632812px;
  }

  100% {
    stroke-dashoffset: 0;
  }
}

@-webkit-keyframes animate-svg-fill-1 {
  0% {
    fill: transparent;
  }

  100% {
    fill: rgb(154, 0, 16);
  }
}

@keyframes animate-svg-fill-1 {
  0% {
    fill: transparent;
  }

  100% {
    fill: rgb(154, 0, 16);
  }
}

.svg-elem-1 {
  -webkit-animation: animate-svg-stroke-1 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0s both,
  animate-svg-fill-1 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 0.8s both;
  animation: animate-svg-stroke-1 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0s both,
  animate-svg-fill-1 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 0.8s both;
}

@-webkit-keyframes animate-svg-stroke-2 {
  0% {
    stroke-dashoffset: 449.749267578125px;
    stroke-dasharray: 449.749267578125px;
  }

  100% {
    stroke-dashoffset: 0;
  }
}

@keyframes animate-svg-stroke-2 {
  0% {
    stroke-dashoffset: 449.749267578125px;
    stroke-dasharray: 449.749267578125px;
  }

  100% {
    stroke-dashoffset: 0;
  }
}

@-webkit-keyframes animate-svg-fill-2 {
  0% {
    fill: transparent;
  }

  100% {
    fill: rgb(4, 0, 0);
  }
}

@keyframes animate-svg-fill-2 {
  0% {
    fill: transparent;
  }

  100% {
    fill: rgb(4, 0, 0);
  }
}

.svg-elem-2 {
  -webkit-animation: animate-svg-stroke-2 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0.12s both,
  animate-svg-fill-2 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 0.9s both;
  animation: animate-svg-stroke-2 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0.12s both,
  animate-svg-fill-2 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 0.9s both;
}

@-webkit-keyframes animate-svg-stroke-3 {
  0% {
    stroke-dashoffset: 1445px;
    stroke-dasharray: 1445px;
  }

  100% {
    stroke-dashoffset: 0;
  }
}

@keyframes animate-svg-stroke-3 {
  0% {
    stroke-dashoffset: 1445px;
    stroke-dasharray: 1445px;
  }

  100% {
    stroke-dashoffset: 0;
  }
}

.svg-elem-3 {
  -webkit-animation: animate-svg-stroke-3 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0.24s both,
  animate-svg-fill-3 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 1s both;
  animation: animate-svg-stroke-3 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0.24s both,
  animate-svg-fill-3 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 1s both;
}
/***************************************************
 * Generated by SVG Artista on 11/22/2020, 11:01:54 PM
 * MIT license (https://opensource.org/licenses/MIT)
 * W. https://svgartista.net
 **************************************************/

svg .svg-elem-1 {
  stroke-dashoffset: 979.4599609375px;
  stroke-dasharray: 979.4599609375px;
  -webkit-transition: stroke-dashoffset 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0s,
  fill 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 0.8s;
  transition: stroke-dashoffset 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0s,
  fill 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 0.8s;
}

svg.active .svg-elem-1 {
  stroke-dashoffset: 0;
}

svg .svg-elem-2 {
  stroke-dashoffset: 1268.5px;
  stroke-dasharray: 1268.5px;
  -webkit-transition: stroke-dashoffset 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0.12s,
  fill 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 0.9s;
  transition: stroke-dashoffset 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0.12s,
  fill 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 0.9s;
}

svg.active .svg-elem-2 {
  stroke-dashoffset: 0;
}

svg .svg-elem-3 {
  stroke-dashoffset: 571.2650146484375px;
  stroke-dasharray: 571.2650146484375px;
  fill: transparent;
  -webkit-transition: stroke-dashoffset 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0.24s,
  fill 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 1s;
  transition: stroke-dashoffset 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0.24s,
  fill 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 1s;
}

svg.active .svg-elem-3 {
  stroke-dashoffset: 0;
  fill: rgb(154, 0, 16);
}

svg .svg-elem-4 {
  stroke-dashoffset: 844.03662109375px;
  stroke-dasharray: 844.03662109375px;
  fill: transparent;
  -webkit-transition: stroke-dashoffset 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0.36s,
  fill 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 1.1s;
  transition: stroke-dashoffset 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0.36s,
  fill 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 1.1s;
}

svg.active .svg-elem-4 {
  stroke-dashoffset: 0;
  fill: rgb(154, 0, 16);
}

svg .svg-elem-5 {
  stroke-dashoffset: 322.7267761230469px;
  stroke-dasharray: 322.7267761230469px;
  fill: transparent;
  -webkit-transition: stroke-dashoffset 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0.48s,
  fill 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 1.2000000000000002s;
  transition: stroke-dashoffset 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0.48s,
  fill 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 1.2000000000000002s;
}

svg.active .svg-elem-5 {
  stroke-dashoffset: 0;
  fill: rgb(154, 0, 16);
}

svg .svg-elem-6 {
  stroke-dashoffset: 225.41241455078125px;
  stroke-dasharray: 225.41241455078125px;
  fill: transparent;
  -webkit-transition: stroke-dashoffset 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0.6s,
  fill 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 1.3s;
  transition: stroke-dashoffset 1s cubic-bezier(0.47, 0, 0.745, 0.715) 0.6s,
  fill 0.7s cubic-bezier(0.47, 0, 0.745, 0.715) 1.3s;
}

svg.active .svg-elem-6 {
  stroke-dashoffset: 0;
  fill: rgb(154, 0, 16);
}

.cls-1, .cls-3 {
  fill: none;
  stroke: #9a0010;
  stroke-miterlimit: 10;
}

.cls-1 {
  stroke-width: 10.24px;
}

.cls-2 {
  opacity: 0.3;
}

.cls-3 {
  stroke-width: 7px;
}

.cls-4 {
  fill: #9a0010;
  fill-rule: evenodd;
}

.cls-5 {
  font-size: 87px;
  fill: #231815;
  font-family: KozGoPr6N-Regular-83pv-RKSJ-H, Kozuka Gothic Pr6N;
}
</style>
