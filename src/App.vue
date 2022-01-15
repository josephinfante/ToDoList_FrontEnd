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
