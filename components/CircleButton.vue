<template>
  <a :href="link" class="btn-circle-border">
    <slot />
  </a>
</template>
<script>
export default {
  props: ['link']
}
</script>
<style scoped>
.btn-circle-border {
  display: inline-block;
  text-decoration: none;
  color: #8B0000;
  width: 150px;
  height: 150px;
  line-height: 150px;
  border-radius: 50%;
  border: solid 2px #8B0000;
  background: #FFFFFF;
  text-align: center;
  overflow: hidden;
  font-weight: bold;
  transition-duration: .4s;
  transition-property: opacity, box-shadow;
}

.btn-circle-border:hover {
  color: #8B0000;
  opacity: 0.5;
  box-shadow: 0 10px 10px;
}
</style>
