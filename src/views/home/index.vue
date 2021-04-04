<template>
  <div class="home">
    <div class="timeline">
      <h1>Home</h1>

      <br />
      <br />

      <Post />

      <br />
      <br />
      <br />

      <Post />
      <br />
      <br />
      <br />
      <Post />
    </div>

    <div class="sidebar">
      <p>
        Lorem ipsum dolor sit amet,sdfgdgbsdgvs
        <br/>
        afsdfasfdafasf
        <br/>
        afsdfasfdafasf
        <br/>
        fdkawoslfkekgfğqwapoekg
      </p>
    </div>
  </div>
</template>

<script>
import Post from '@/components/Post'
export default {
  name: 'Home',
  components: { Post }
}
</script>

<style lang="scss" scoped>
.home {
  max-width: none;
  margin-left: auto;
  margin-right: auto;
  display: grid;  
  grid-template-columns: 1fr 295px;
  grid-gap: 30px;
}

.sidebar {
  display: block;
}
</style>
