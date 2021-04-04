<template>
  <div class="home">
    <CustomText tag="h1">Profile Post</CustomText>
    <Post />
  </div>
</template>

<script>
import CustomText from '@/components/CustomText'
import Post from '@/components/Post'

export default {
  name: 'ProfilePost',
  components: {
    CustomText,
    Post
  }
}
</script>

<style scoped></style>
