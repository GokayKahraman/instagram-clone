<template>
  <div class="post">
    <header class="header section">
      <div class="header-author">
        <Avatar :size="40" />
        <div class="header-author-info">
          <div>
            <CustomText tag="b">gokykh</CustomText>
          </div>
          <div>
            <CustomText size="xsmall">Çorlu, Tekirdağ</CustomText>
          </div>
        </div>
      </div>
      <div class="header-more">
        <button type="button">
          <IconMore />
        </button>
      </div>
    </header>

    <div class="post-media">
      <img
        src="https://instagram.fist13-1.fna.fbcdn.net/v/t51.2885-19/s150x150/129741738_2660165120960418_335456544425767077_n.jpg?tp=1&_nc_ht=instagram.fist13-1.fna.fbcdn.net&_nc_ohc=PRQkPOcjY64AX-KhYKC&edm=ABfd0MgAAAAA&ccb=7-4&oh=f023b88c128441875a2eb199723b95aa&oe=608DDAB8&_nc_sid=7bff83"
        alt=""
      />
    </div>

    <div class="action-buttons section">
      <button type="button">
        <IconLike />
      </button>
      <button type="button">
        <IconComment />
      </button>
      <button type="button">
        <IconDirect />
      </button>
      <button class="action-save" type="button">
        <IconSave />
      </button>
    </div>

    <div class="view-count section">
      <custom-text tag="b">1.345 beğenme</custom-text>
    </div>
  </div>
</template>

<script>
import Avatar from '@/components/Avatar'
import CustomText from '@/components/CustomText'
import IconMore from '@/assets/icons/more.svg'
import IconLike from '@/assets/icons/like.svg'
import IconComment from '@/assets/icons/comment.svg'
import IconDirect from '@/assets/icons/direct.svg'
import IconSave from '@/assets/icons/save.svg'

export default {
  name: 'Post',
  components: {
    IconLike,
    IconComment,
    IconDirect,
    IconSave,
    IconMore,
    CustomText,
    Avatar
  }
}
</script>

<style lang="scss" scoped>
.post {
  border-radius: 3px;
  
}

.section {
  padding-left: 16px;
  padding-right: 16px;
}

.header {
  height: 60px;
  display: flex;
  align-items: center;

  &-author {
    display: flex;
    align-items: center;

    &-info {
      margin-left: 8px;
    }
  }

  &-more {
    margin-left: auto;
  }
}

.action-buttons {
  height: 45px;
  display: flex;
  align-items: center;

  button {
    margin-right: 16px;
  }

  .action-save {
    margin-left: auto;
    margin-right: 0;
  }
}
</style>
