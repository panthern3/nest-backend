<template>
    <section class="top bg-gradient-to-b from-gray-900 to-gray-800 py-16 px-8 lg:px-60">
    <div class="container mx-auto my-auto">
      <div class="flex-col-reverse lg:flex-row jusify-between space-y-8 lg:space-y-0 lg:space-x-8 lg:items-center lg:relative right-8 flex">
        <article class="left flex flex-col justify-center lg:w-1/2 py-8 px-4 md:px-8 lg:px-16 lg:mr-auto mg-8 lg:mb-0">
          <div class="">
            <h2 class="text-4xl font-bold text-white mb-4">We do campaigns that works well for your idea</h2>
            <p class="text-white text-lg mb-4">Our documentary campaigns feature leading figures, organisations and leaders, in open and candid discussions about transformative strategies and mindsets. Addressing complex trends.</p>
          </div>
          <button class="text-left w-40 text-transparent bg-gradient-to-r from-purple-600 to-indigo-600 bg-clip-text font-bold rounded">All campaigns</button>
          <figure class="relative bottom-0.5 left-1">
            <img src="arrow.svg" class="w-3 h-3 relative left-28 bottom-4" alt="arrow">
          </figure>
        </article>
        <figure class="right lg:w-1/2 lg:ml-auto mb-8 lg:mb-0">
          <img src="right.jpg" alt="Изображение" class="w-full rounded-3xl">
        </figure>
      </div>
      <div class="flex flex-col lg:flex-row mt-16 lg:relative left-8">
        <figure class="left lg:w-1/2">
          <img src="left.jpg" alt="Изображение" class="w-full rounded-3xl">
        </figure>
        <article class="right flex flex-col justify-center lg:w-1/2 py-8 px-4 md:px-8 lg:px-16">
          <div class="">
            <h2 class="text-4xl font-bold text-white mb-4">We make films that stick in your heart</h2>
            <p class="text-white text-lg mb-4">This exclusive service provided by our team of professional content creators is available for global use. Our clients will have access and total creative control throughout the process of production, with resources and talent supplied by us.</p>
          </div>
          <button class="text-left w-44 text-transparent bg-gradient-to-r from-purple-600 to-indigo-600 bg-clip-text font-bold rounded">I have an idea for film</button>
          <figure class="relative bottom-0.5 right-0.5">
            <img src="arrow.svg" class="w-3 h-3 relative left-44 bottom-4" alt="arrow">
          </figure>
        </article>
      </div>
    </div>
    </section>
  </template>
  
  <script>
  export default {
  }
  </script>
  
  <style scoped>
  h2 {
    font-family: 'Arboria-Medium';
  }

  p {
    font-family: 'Arboria-Book';
  }

  button {
    font-family: 'Arboria-Medium';
  }
  
</style>