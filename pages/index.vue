<template>
  <div>
    <div class="mx-auto" style="width: 200px;">
      <canvas id="myChartc" class="my-4 w-100" width="900" height="400" />
    </div>
    <div class="text-center">
      <Logo />
      <canvas id="myChartb" class="my-4 w-100" width="900" height="50" />
      <circle-button link="/origin">
        What's Inovange
      </circle-button>
      <circle-button link="/member">
        members
      </circle-button>
      <circle-button link="/portforio">
        works
      </circle-button>
    </div>
  </div>
</template>
<script>
import Logo from '@/components/Logo'
import CircleButton from '~/components/CircleButton'

export default {
  components: { CircleButton, Logo }
}
</script>
<style>
</style>
