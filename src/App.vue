<template>
  <div>
    <Header />
    <div class="container mx-auto min-h-screen text-center pt-10">
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
  src: local('Poppins-regular'), url('./assets/fonts/Poppins/Poppins-Regular.ttf');
}
@font-face {
  font-family: 'Poppins-medium';
  src: local('Poppins-medium'), url('./assets/fonts/Poppins/Poppins-Medium.ttf');
}
@font-face {
  font-family: 'Poppins-semibold';
  src: local('Poppins-semibold'), url('./assets/fonts/Poppins/Poppins-SemiBold.ttf');
}
@font-face {
  font-family: 'Poppins-black';
  src: local('Poppins-black'), url('./assets/fonts/Poppins/Poppins-Black.ttf');
}
* {
  font-family: 'Poppins-regular';
}
h1 {
  font-family: 'Poppins-black';
}
</style>