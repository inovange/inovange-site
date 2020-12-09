<template>
  <div>
    <div class="mx-auto" style="width: 200px;">
      <canvas class="my-4 w-100" id="myChartc" width="900" height="400"></canvas>
    </div>
    <div>
      <Logo/>
      <canvas class="my-4 w-100" id="myChartb" width="900" height="50"></canvas>
     <center>
       <a href="#" class="btn-circle-border-simple">What's Inovange</a>
      <a href="#" class="btn-circle-border-simple">members</a>
      <a href="#" class="btn-circle-border-simple">works</a>
     </center>
    </div>
  </div>
</template>
<script>
import Logo from '@/components/Logo'

export default {
  components: { Logo }
}
</script>
<style>
.btn-circle-border-simple {
  display: inline-block;
  text-decoration: none;
  color: #8B0000;
  width: 150px;
  height: 150px;
  line-height: 150px;
  border-radius: 50%;
  border: solid 2px #8B0000;
  text-align: center;
  overflow: hidden;
  font-weight: bold;
  transition: .4s;
}

.btn-circle-border-simple:hover {
  background: #FFFFFF;
}
</style>
