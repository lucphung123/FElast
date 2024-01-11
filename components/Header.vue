<template>
  <div class="w-full flex flex-col justify-center items-center">
    <div class="w-full">
      <div class="w-full flex justify-between items-center">
        <div class="flex">
          <nuxt-link to="/" class="">
            <img src="/logo1.png" class="object-contain w-40 h-30" alt="" />
          </nuxt-link>
          <div class="flex items-center mt-5 gap-10">
            <p class="text-xl font-600 cursor-pointer hover:text-#004390">Trang chủ</p>
            <div class="relative inline-block text-left">
              <p @click="toggleDropdown" class="text-xl font-600 cursor-pointer hover:text-#004390">Sản phẩm</p>
              <div v-if="isDropdownOpen" class="dropdown origin-top-right absolute -right-20 mt-2 w-48 rounded-md shadow-lg bg-white ring-1 ring-black ring-opacity-5">
                <p class="block cursor-pointer px-4 py-2 text-sm text-gray-700 hover:bg-gray-100 hover:text-gray-900">Sách Tiếng Việt</p>
                <p class="block cursor-pointer px-4 py-2 text-sm text-gray-700 hover:bg-gray-100 hover:text-gray-900">Sách Tiếng Anh</p>
                <p class="block cursor-pointer px-4 py-2 text-sm text-gray-700 hover:bg-gray-100 hover:text-gray-900">Manga - Comic</p>
              </div>
            </div>
            <p class="text-xl font-600 cursor-pointer hover:text-#004390">Tin tức</p>
            <p class="text-xl font-600 cursor-pointer hover:text-#004390">Liên hệ</p>
          </div>
        </div>
        <div>
          <div class="flex gap-5 items-center">
            <div class="relative">
              <input type="text" placeholder="Nhập từ khóa...." class="rounded-full bg-gray-200 h-40px w-250px px-5 text-sm" />
              <div class="i-mdi:magnify absolute text-2xl top-2 right-3"></div>
            </div>
            <div class="i-mdi:cart text-2xl"></div>
            <button class="text-#004390 rounded-full h-40px w-130px font-bold text-sm border-none hover:(bg-#f1b821 text-black)">ĐĂNG KÝ</button>
            <button class="text-white bg-#004390 rounded-full h-40px w-130px font-bold text-sm border-none hover:(bg-#f1b821 text-black)">ĐĂNG NHẬP</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
import { ref } from "vue"

const isDropdownOpen = ref(false)

const toggleDropdown = () => {
  isDropdownOpen.value = !isDropdownOpen.value
}
</script>
