<template>
  <div class="font-pvh fixed bg-gray-100 top-0 left-0 right-0 flex h-16 p-2 mb-4 border-b border-gray-300" >
    <div class="flex-none w-12 h-12">
      <router-link to="/dashboard">
        <img src="./../../assets/logo.png" class="w-full rounded-full p-1 bg-gray-100" alt="SCT Logo" title="SCT Logo" />
      </router-link>
    </div>
    <div class="flex-grow h-12 text-lg leading-10 text-left pl-4 pt-1 font-muol ">
      ប្រព័ន្ធគ្រប់គ្រងការលក់ដូរ
    </div>
    <div class="flex-none w-32 h-10 py-1 mr-2 leading-10 text-right">
      <div class="w-32 ">{{ username }}</div>
    </div>
    <div class="flex-none w-12 h-12 cursor-pointer ">
      <!-- <div class="w-12 h-12 rounded-full" >
        <svg v-if="profilePicture==null" xmlns="http://www.w3.org/2000/svg" class="w-12 h-12" fill="none" viewBox="0 0 24 24" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5.121 17.804A13.937 13.937 0 0112 16c2.5 0 4.847.655 6.879 1.804M15 10a3 3 0 11-6 0 3 3 0 016 0zm6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
        </svg>
        <img v-if="profilePicture!==null" :src="profilePicture" />
      </div> -->
    </div>
  </div>
</template>

<script >
import { computed } from 'vue'
import { getUser } from './../../plugins/authentication'
export default {
  name: 'Topmenu'  ,
  setup(){
    const username = computed(() => {
      let user = getUser()
      return user !== null ? user.name : "" 
    })

    const profilePicture = computed(() => {
      let user = getUser()
      return user !== null && user.avatar_url !== null ? user.avatar_url : null 
    })
    
    return {
      username ,
      profilePicture
    }
  }
}
</script>