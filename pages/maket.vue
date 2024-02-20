<template>
  
    <div>
      <Nav />
      <maketFigma />
    </div>
  </template>
  
  
  <script>
  import Nav from '@/components/Nav.vue';
  import maketFigma from '@/components/maketFigma.vue';


  export default {
    components: {
      Nav,
      maketFigma
    }
  };
  </script>