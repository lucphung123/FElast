<template>
  <div class="w-full flex flex-col justify-center items-center">
    <div class="w-full">
      <div class="w-full flex justify-between items-center">
        <div class="flex ">
          <nuxt-link to="/" class="">
            <img src="/logo1.png" class="object-contain w-40 h-30" alt="" />
          </nuxt-link>
          <div class="flex gap-5 mt-15">
            <p class="text-lg font-600 cursor-pointer hover:text-#004390 mt-4">Sách Tiếng Việt</p>
            <p class="text-lg font-600 cursor-pointer hover:text-#004390 mt-4">Sách Tiếng Anh</p>
            <p class="text-lg font-600 cursor-pointer hover:text-#004390 mt-4">Manga - Comic</p>
          </div>
        </div>
        <div>
          <div class="flex justify-end items-center gap-10">
            <div class="flex items-center gap-2">
              <div class="i-mdi:phone  text-2xl"></div>
              <div class="font-bold text-4">
                <p>0987654321</p>
              </div>
            </div>
            <div class="i-mdi:cart text-2xl">
            </div>

          </div>
          <div class="flex gap-5">
            <div class="relative">
              <input type="text" placeholder="Nhập từ khóa...." class="rounded-full bg-gray-200 h-40px w-250px px-5 text-sm" />
              <div class="i-mdi:magnify absolute text-2xl top-2 right-3"></div>
            </div>
            <button class="text-#004390 rounded-full h-40px w-130px font-bold text-sm border-none hover:(bg-#f1b821 text-black)">ĐĂNG KÝ</button>
            <button class="text-white bg-#004390 rounded-full h-40px w-130px font-bold text-sm border-none hover:(bg-#f1b821 text-black)">ĐĂNG NHẬP</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
