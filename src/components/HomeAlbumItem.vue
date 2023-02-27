<script setup>
import Duration from 'duration-js';
</script>

<script>
export default {
    props: ['video']
}
</script>

<template>
    <div class="col">
        <div class="card shadow-sm">
            <svg class="bd-placeholder-img card-img-top" width="100%" height="225" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Placeholder: Thumbnail" preserveAspectRatio="xMidYMid slice" focusable="false"><title>Placeholder</title><rect width="100%" height="100%" fill="#55595c"/><text x="50%" y="50%" fill="#eceeef" dy=".3em">Thumbnail</text></svg>

            <div class="card-body">
                <h5>{{ video.title }}</h5>
                <p class="card-text">{{ this.video.description }}</p>
                <div class="d-flex justify-content-between align-items-center">
                    <div class="btn-group">
                        <RouterLink class="btn btn-sm btn-outline-secondary" to="/watch">
                            View
                        </RouterLink>
                    </div>
                    <small class="text-muted">{{ this.video.duration }}</small>
                </div>
            </div>
        </div>
    </div>
</template>
