<template>
  <div class="flex flex-col items-center space-y-4 mt-10">
    <i class="fa-brands fa-twitter text-4xl text-primary"></i>
    <span class="text-2xl font-bold">포폴용 회원가입</span>
    <input v-model="username" type="text" class="w-96 px-4 py-3 rounded border border-gray-300 focus:ring-2 focus:border-primary resize-none focus:outline-none" placeholder="이메일">
    <input v-model="email" type="text" class="w-96 px-4 py-3 rounded border border-gray-300 focus:ring-2 focus:border-primary resize-none focus:outline-none" placeholder="아이디">
    <input v-model="password" type="password" class="w-96 px-4 py-3 rounded border border-gray-300 focus:ring-2 focus:border-primary resize-none focus:outline-none" placeholder="비밀번호">
    <button class="w-96 rounded-full bg-primary text-white py-3 hover:bg-dark" @click="onregister">회원가입</button>
    <button class="text-primary">계정이 이미 있으신가요? 로그인 하기</button>
  </div>
</template>

<script>
import { ref } from 'vue';

export default {
    setup(){
        const username = ref('');
        const email = ref('');
        const password = ref('');
        const loading = ref(false);

        const onregister = () =>{
            console.log(username.value,email.value,password.value);
        }

        return{
            username,
            email,
            password,
            onregister,
            loading
        }
    }

}
</script>

<style>

</style>