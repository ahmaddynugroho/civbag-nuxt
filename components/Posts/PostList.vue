<template>
  <section class="post-list">
      <PostPreview 
        id="1"
        :is-admin="isAdmin"
        thumbnail="https://mobileague.id/wp-content/uploads/2020/02/arknights-indonesia.jpg"
        title="Hello There"
        previewText="This is my first post!"
      />
      <PostPreview 
        id="2"
        :is-admin="isAdmin"
        thumbnail="https://encdn.ldmnq.com/emulator/arknights.jpg"
        title="Hello There - the second time"
        previewText="This is my second post!"
      />
      <PostPreview 
        id="3"
        :is-admin="isAdmin"
        thumbnail="https://nawalakarsa.id/wp-content/uploads/2020/03/Arknights-Low-Rarity-Header.jpg"
        title="Hi!"
        previewText="This is my third post!"
      />
    </section>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'

export default {
  components: {
    PostPreview
  },
  props: {
    isAdmin: {
      type: Boolean,
      default: false
    }
  }
}
</script>

<style scoped>
.post-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>