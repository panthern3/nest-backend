<template>
  
  <div>
    <Nav />
    <Form />
  </div>
</template>


<script>
import Form from '@/components/Form.vue';
import Nav from '@/components/Nav.vue';

export default {
  components: {
    Form,
    Nav
  }
};
</script>