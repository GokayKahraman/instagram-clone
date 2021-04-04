<template>
  <header class="header">
    <Container class="header-inner">
      <router-link to="/" class="logo">
        Instagram
      </router-link>

      <!-- search -->
      <form class="search">
        <input type="text" placeholder="Search" />
      </form>

      <!-- navigation -->
      <nav class="navigation">
        <router-link to="/">
          <IconHomeFill v-if="$route.name === 'Home'" />
          <IconHome v-else />
        </router-link>
        <router-link to="/direct">
          <IconDirectFill v-if="$route.name === 'Direct'" />
          <IconDirect v-else />
        </router-link>
        <router-link to="/explore">
          <IconExploreFill v-if="$route.name === 'Explore'" />
          <IconExplore v-else />
        </router-link>
        <router-link to="/profile">
          <Avatar size="26" />
        </router-link>
      </nav>
    </Container>
  </header>
</template>

<script>
import IconHome from '@/assets/icons/home.svg'
import IconHomeFill from '@/assets/icons/home-fill.svg'
import IconDirect from '@/assets/icons/direct.svg'
import IconDirectFill from '@/assets/icons/direct-fill.svg'
import IconExplore from '@/assets/icons/explore.svg'
import IconExploreFill from '@/assets/icons/explore-fill.svg'
import Container from '@/components/Container'
import Avatar from '@/components/Avatar'

export default {
  name: 'MainHeader',
  components: {
    Avatar,
    Container,
    IconHome,
    IconHomeFill,
    IconDirect,
    IconDirectFill,
    IconExplore,
    IconExploreFill
  }
}
</script>

<style lang="scss" scoped>

.header {
  z-index: 90;
  position: fixed;
  left: 0;
  right: 0;
  top: 0;
  border-bottom: 1px solid rgba(var(--b6a),1);
  background-color: white;
}

.header-inner {
  height: var(--header-height);
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  align-items: center;
  justify-content: center;
}

.logo {
  font-size: 1.6rem;
  font-weight: bold;
}

.search {
  display: block;
  text-align: center;

  input {
      width: 215px;
      height: 28px;
      border: 1px solid rgba(var(--b6a),1);
      background-color: rgba(var(--b3f),1);
      border-radius: 4px;
      padding-left: 20px;
      padding-right: 20px;
    }
}
.navigation {
  z-index: 90;
  position: static;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: white;
  border: 0;
  border-top: 1px solid white;
  height: auto;
  display: flex;
  align-items: center;
  justify-content: flex-end;

  a {
      margin-left: 20px;
    }

}
</style>
