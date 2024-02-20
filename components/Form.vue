<template>
    <div class="flex items-center justify-content h-screen">
      <form @submit.prevent="submitForm" class="max-w-md mx-auto">
        <div class="mb-4">
          <label for="fullname" class="block text-gray-700 text-sm font-bold mb-2">Имя Фамилия</label>
          <input v-model="fullname" placeholder="Введите ваше имя:" type="text" id="fullname" name="fullname" :class="{ 'border-red-500': fullnameError }" class="transition duration-500 bg-gray-100 hover:bg-gray-200 shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline">
          <p v-if="fullnameError" class="text-red-500 text-xs italic">Пожалуйста, введите кириллицей имя и фамилию.</p>
        </div>
        <div class="mb-4">
          <label for="phone" class="block text-gray-700 text-sm font-bold mb-2">Номер телефона</label>
          <input v-model="phone" placeholder="+7 *** *** ** **" type="text" id="phone" name="phone" :class="{ 'border-red-500': phoneError }" class="transition duration-500 bg-gray-100 hover:bg-gray-200 shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline">
          <p v-if="phoneError" class="text-red-500 text-xs italic">Пожалуйста, введите номер начинающийся с +7.</p>
        </div>
        <div class="mb-4">
          <label for="email" class="block text-gray-700 text-sm font-bold mb-2">Email</label>
          <input v-model="email" placeholder="username@domen.com" type="email" id="email" name="email" class="transition duration-500 bg-gray-100 hover:bg-gray-200 shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline">
         </div>
        <div class="mb-4">
          <label for="password" class="block text-gray-700 text-sm font-bold mb-2">Пароль</label>
          <input v-model="password" placeholder="Введите ваш пароль:" type="password" id="password" name="password" class="transition duration-500 bg-gray-100 hover:bg-gray-200 shadow appearance-none border rounded w-full py-2 px-3 text-gray-700 leading-tight focus:outline-none focus:shadow-outline">
        </div>
        <div class="mb-4">
          <button type="submit" class="transition duration-500 bg-red-500 hover:bg-red-700 text-white font-bold py-2 px-4 rounded focus:outline-none focus:shadow-outline">Отправить</button>
        </div>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        fullname: '',
        phone: '',
        email: '',
        password: '',
        fullnameError: false,
        phoneError: false
      };
    },
    methods: {
      submitForm() {
        const fullnamePattern = /^[а-яА-ЯёЁ\s]+$/;
        if (!fullnamePattern.test(this.fullname)) {
          this.fullnameError = true;
          return;
        } else {
          this.fullnameError = false;
        }
  
        const phonePattern = /^\+?\d{10,14}$/;
        if (!phonePattern.test(this.phone)) {
          this.phoneError = true;
          return;
        } else {
          this.phoneError = false;
        }
  
        console.log('Отправка данных:', {
          fullname: this.fullname,
          phone: this.phone,
          email: this.email,
          password: this.password
        });
      }
    }
  };
  </script>
  
  <style>
  </style>