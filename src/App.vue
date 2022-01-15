<template>
  <div>
    <Header />
    <div class="bg-red-500 container mx-auto min-h-screen text-center">
      <router-view/>
    </div>
  </div>
</template>

<script>
import './assets/tailwind.css';
import Header from '@/components/Header';

export default {
  components: {
    Header
  }  
}
</script>

<style>
@font-face {
  font-family: 'Poppins-regular';
  src: local('Poppins-regular'), url('./assets/fonts/Poppins-Regular.ttf');
}
</style>