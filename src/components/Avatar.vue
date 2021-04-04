<template>
  <figure class="avatar">
    <img :src="src" :alt="alt" :width="size" :height="size" />
  </figure>
</template>

<script>
export default {
  name: 'Avatar',
  props: {
    src: {
      type: String,
      default:
        'https://instagram.fist13-1.fna.fbcdn.net/v/t51.2885-19/s150x150/129741738_2660165120960418_335456544425767077_n.jpg?tp=1&_nc_ht=instagram.fist13-1.fna.fbcdn.net&_nc_ohc=PRQkPOcjY64AX-KhYKC&edm=ABfd0MgAAAAA&ccb=7-4&oh=f023b88c128441875a2eb199723b95aa&oe=608DDAB8&_nc_sid=7bff83'
    },
    alt: {
      type: String
    },
    size: {
      type: Number
    }
  }
}
</script>

<style lang="scss" scoped>
.avatar {
  display: inline-flex;
  padding: 2px;
  border-radius: 999px;
  background: linear-gradient(
    219deg,
    rgba(184, 63, 140, 1) 0%,
    rgba(237, 158, 90, 1) 100%
  );

  img {
    border-radius: inherit;
    border: 2px solid white;
  }
}
</style>
