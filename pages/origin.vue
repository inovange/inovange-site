<template>
  <div class="text">
    <h1>
      Inovangeとは
    </h1>
    <div id="console" />

    <p class="bold">
      <br><br><br><br>
    </p>
    <p class="art">
      イノベーション（革新）×チャレンジ（挑戦）→イノベンジ 挑戦し革新し続ける
    </p>
    <br><br>

    <p>
      <img class="logo" src="/logo.png" alt="inovangeロゴ" />
    </p>
    <p class="write-text" :style="style">{{text}}</p>
    <br><br><br>
    <h1 class="abc">
      "これが私たち"
    </h1>
    <br><br><br><br><br><br><br>
    そんな私たちInovangeの使命は人々に「揺らぎ」を与えること
    <br>
    それが私たちの役割です
    <p class="future">
      これからの”webデザイン”を
      私が”革新”に”挑戦”し続けることは使命です。
    </p>
    <p>
      革新→揺れる→つながる<br><br><br>
      私たちの革新×挑戦によって人が同じ波長で揺れた時人々はつながります。
      Inovangeではまずwebデザインで革新を起こします。
      Inovangeでは革新を起こすにふさわしい個性的なメンバーが揃っています。
      こいつらに常識は通用しません。
      常識に”挑戦”し”革新”を起こすwebデザインを見ていってください！！！
    </p>
  </div>
</template>

<script>

export default {
  head () {
    return {
      title: "what's Inovange",
      meta: [
        { hid: 'description', name: 'description', content: 'description' }
      ]
    }
  },
  data () {
    return {
      text: '',
      style: {}
    }
  },
  mounted () {
    const words = ['これが私たち.']
    const colors = ['tomato']
    let visible = true
    let letterCount = 1
    let x = 1
    let waiting = false
    this.style.color = colors[0]
    window.setInterval(() => {
      if (letterCount === 0 && waiting === false) {
        waiting = true
        this.text = words[0].substring(0, letterCount)
        window.setTimeout(() => {
          colors.push(colors.shift())
          words.push(words.shift())
          x = 1
          this.style.color = colors[0]
          letterCount += x
          waiting = false
        }, 1000)
      } else if (letterCount === words[0].length + 1 && waiting === false) {
        waiting = true
        window.setTimeout(function () {
          x = -1
          letterCount += x
          waiting = false
        }, 1000)
      } else if (waiting === false) {
        this.text = words[0].substring(0, letterCount)
        letterCount += x
      }
    }, 120)
    window.setInterval(function () {
      visible = !visible
    }, 400)
  }
}

</script>

<style>
.abc {
  color: #9A0010;
}
.write-text {
  height: 1em;
}
.text {
  text-align: center;
  min-height: 100vh;
  font-size: x-large;
}

.logo {
  width: 720px;
  max-width: 100%;
}

.future {
  color: #fff;
  text-shadow: 1px 1px 1px #ff9800, -1px 1px 1px #ff9800, 1px -1px 1px #ff9800, -1px -1px 1px #ff9800, 1px 1px 1px #ff9800, -1px 1px 1px #ff9800, 1px -1px 1px #ff9800, -1px -1px 1px #ff9800;
}

.art {
  color: #00BCD4;
  text-shadow: 2px 2px #fff, 5px 5px rgba(0, 188, 212, 0.4);
}
</style>
