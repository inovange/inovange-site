<template>
  <div class="container main">
    <div class="home tag">
      <span>Home</span>
    </div>

    <div class="containert">
      <h1>Member</h1>
    </div>

    <div class="container1">
      <div class="container-i-1">
        <img src="../static/jm-dav-dhAgfU99RCs-unsplash.jpg" height="200" width=""/>
      </div>
      <div class="container-t-1">
        <p>アイウエオ</p>
      </div>

    </div>
    <div class="container2">
      <img src="/thomas-yohei-0fjRZf08HJQ-unsplash.jpg" height="300" width=""/>
    </div>
    <div class="container3">
      <img src="/ben-klewais-APi5Pa4bEcI-unsplash.jpg" height="300" width=""/>
    </div>
    <div class="container4">
      <img src="/michael-bowman-GVMdjXsFpXo-unsplash.jpg" height="200" width=""/>
    </div>
  </div>

</template>

<script>
export default {}
</script>

<style>
span {
  border: 1px solid;
  border-color: #35495e;
}

h1 {
  position: absolute;
  left: 50%;
  top: 50%;
  font-size: 50px;
  transform: translate(-50%,-50%);
}

.containert {
  display: flex;
  height: 500px;
  width: auto;
  position: relative;

}

.container-i-1 {
  width: 50%;
  float: left;
}

.container-t-1 {
  width: 50%;
  float: left;
}

.container1 {
  margin: 0 auto;
  border: 2px solid black;
  width: 100%;
  height: 400px;
}

.container2 {
  margin-top: 100px;
  border: 2px solid black;
  width: auto;
  height: 400px;
}

.container3 {
  margin-top: 100px;
  border: 2px solid black;
  width: auto;
  height: 400px;
}

.container4 {
  margin-top: 100px;
  border: 2px solid black;
  width: auto;
  height: 400px;
}
</style>
