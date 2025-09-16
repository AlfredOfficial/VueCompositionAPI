<script setup>
import PostItem from '@/components/PostItem.vue';
import Wrapper from '@/components/Wrapper.vue';
import { usePostsStore } from '@/stores/posts';

const postStore = usePostsStore();
</script>

<template>
  <!-- <main> -->
    <div class="header">
      <div>
        <h4>All Posts</h4>
      </div>
      <button>Show saved Posts</button>
    </div>

    <div v-for="post in postStore.sorted" :key="post.id">
      <Wrapper>
        <PostItem :post="post"/>
      </Wrapper>
    </div>
  <!-- </main> -->
</template>

<style lang="scss" scoped>
// Example SCSS for your posts header section

.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 2rem;
  padding: 1rem 2rem;
  position: sticky;
  top: 56px;
  background: #fff;
  z-index: 10;

  > div {
    h4 {
      font-size: 1.5rem;
      font-weight: 600;
      color: #333;
      margin: 0;
    }
  }

  button {
    background: #4f8cff;
    color: #fff;
    border: none;
    border-radius: 6px;
    padding: 0.5rem 1.2rem;
    font-size: 1rem;
    cursor: pointer;
    transition: background 0.2s;

    &:hover {
      background: #2563eb;
    }
  }
}
</style>