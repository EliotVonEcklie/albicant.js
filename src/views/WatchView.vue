<script setup>
import VideoPlayer from '../components/VideoPlayer.vue';
</script>
<script>
export default {
    data() {
        return {
            videoOptions: {
                autoplay: true,
                controls: true,
                sources: [
                    {
                        src: 'https://download.samplelib.com/mp4/sample-30s.mp4',
                        type: 'video/mp4'
                    }
                ]
            },
            videoUrl: 'https://download.samplelib.com/mp4/sample-30s.mp4'
        };
    }
};
</script>

<template>
    <h1 class="px-3">Watch</h1>

    <main>
        <div class="w-[768px] h-[400px]">
            <video width="768" height="400" :src="videoUrl" controls></video>
        </div>
    </main>
</template>
