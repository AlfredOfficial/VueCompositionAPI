<!-- <script setup>
import { RouterLink, RouterView } from 'vue-router'
import { usePostsStore } from '@/stores/posts';
const postStore = usePostsStore();

postStore.getPosts();

</script>

<template>
  <header>
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/add-post">Add Post</RouterLink>
      </nav>
  </header>

  <RouterView />
</template>


<style lang="scss" scoped>
header {
  position: sticky;
  top: 0;
  z-index: 100;
  background-color: #90caf9;
}

nav {
  padding: 1rem 2rem;
  border-bottom: 1px solid #90caf9;
}

nav a {
  color: #fff;
  padding: 5px 15px;
  border-radius: 5px;
  transition: all 0.2s ease-in-out;
  margin-right: 1rem;
  text-decoration: none;
}

nav a:hover {
  background-color: #64b5f6;
}
</style> -->

<script setup>
import { RouterLink, RouterView } from 'vue-router'
import { usePostsStore } from '@/stores/posts';
const postStore = usePostsStore();

postStore.getPosts();
</script>

<template>
  <header>
    <nav>
      <div class="nav-logo">
        <!-- Replace with an <img> if you want a logo image -->
        <span class="logo-text">VueCompAPI</span>
      </div>
      <div class="nav-links">
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/add-post">Add Post</RouterLink>
      </div>
    </nav>
  </header>

  <RouterView />
</template>

<style lang="scss" scoped>
header {
  position: sticky;
  top: 0;
  z-index: 100;
  background-color: #90caf9;
}

nav {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 1rem 2rem;
  border-bottom: 1px solid #90caf9;
}

.nav-logo {
  font-weight: bold;
  font-size: 1.3rem;
  color: #fff;
  letter-spacing: 1px;
}

.nav-links {
  display: flex;
  align-items: center;
}

.nav-links a {
  color: #fff;
  padding: 5px 15px;
  border-radius: 5px;
  transition: all 0.2s ease-in-out;
  margin-right: 1rem;
  text-decoration: none;
}

.nav-links a:last-child {
  margin-right: 0;
}

.nav-links a:hover {
  background-color: #64b5f6;
}
</style>