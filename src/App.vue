<script setup>
import { RouterLink, RouterView } from 'vue-router';
import 'bootstrap';
import 'bootstrap/dist/css/bootstrap.min.css';
</script>

<template>
  <header>
    <div class="wrapper">
      <nav class="nav nav-pills p-2">
        <RouterLink to="/" class="nav-item nav-link" active-class="active">
          Home
        </RouterLink>
        <RouterLink to="/about" class="nav-item nav-link" active-class="active">
          About
        </RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>
