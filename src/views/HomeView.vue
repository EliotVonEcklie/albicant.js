<script setup>
import HomeAlbumItem from '../components/HomeAlbumItem.vue';
</script>
<script>
export default {
    data() {
      return {
        video_test: [
          {
            id: 0,
            title: 'Hello',
            description: 'Lorem Ipsum',
            duration: '9 seconds'
          },
          {
            id: 1,
            title: 'World',
            description: 'Dolor Sit',
            duration: '10 hours'
          }
        ]
      }
    }
}
</script>

<template>
    <main>
        <div class="album py-5 bg-light">
            <div class="container">
                <div class="row row-cols-1 row-cols-sm-2 row-cols-md-3 g-3">
                    <HomeAlbumItem v-for="video in video_test" :key="video.id" :video="video"/>
                </div>
            </div>
        </div>
    </main>
</template>

<style>
.bd-placeholder-img {
  font-size: 1.125rem;
  text-anchor: middle;
  -webkit-user-select: none;
  -moz-user-select: none;
  user-select: none;
}
</style>
