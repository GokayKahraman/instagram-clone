<template>
  <div>
    <CustomText class="a1" tag="p">hello vue</CustomText>
    <CustomText class="a2" tag="p" size="small">hello vue</CustomText>
    <CustomText class="a3" tag="p" size="xsmall">hello vue</CustomText>
    <IconHome />
  </div>
</template>

<script>
import CustomText from './components/CustomText'
import IconHome from './assets/icons/home.svg'

export default {
  name: 'Home',
  components: {
    CustomText,
    IconHome
  }
}
</script>

<style scoped>
.a1 {
  color: rgba(var(--ba8), 0.5);
}
.a2 {
  color: rgb(var(--cdd));
}
.a3 {
  color: rgb(var(--ba8));
}
</style>
