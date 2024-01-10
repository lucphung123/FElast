<template>
  <div class="my-20 w-full space-y-10">
    <div class="flex items-center">
      <div class="i-mdi:bookmark-outline text-4xl bg-blue-900"></div>
      <p class="text-#004390 font-700 text-3xl">TIN TỨC & SỰ KIỆN</p>
    </div>
    <div class="flex">
      <div v-for="items in newsItems.slice(0, 1)" :key="items.id" class="w-full lg:w-3/5 px-3 animate-bounce-in-left animate-duration-1.5s">
        <img @click="router_push(newsItems[0].slug)" :src="items.image" alt="" class="w-full cursor-pointer h-auto rounded-md object-cover" />
        <div class=" w-30 flex mt-3 justify-center bg-yellow-500 rounded-md">
          <p class="text-lg cursor-pointer text-white">28/06/2023</p>
        </div>
        <p class="mt-3 text-lg cursor-pointer md:text-xl text-blue-800 font-bold">{{ items.title }}</p>
      </div>
      <div>
        <div @click="router_push(items.slug)" v-for="items in newsItems.slice(1, 4)" :key="items.id" class="flex md:space-x-5 flex-col md:flex-row mb-5 px-3 animate-bounce-in-right animate-duration-1.5s">
          <div class="w-full md:w-300px h-auto md:h-150px">
            <img :src="items.image" alt="" class="w-full h-full rounded-md object-cover cursor-pointer" />
          </div>
          <div class="w-full md:w-300px">
            <div class=" w-30 mt-3 md:mt-0 flex justify-center bg-yellow-500 rounded-md cursor-pointer">
              <p class="text-lg text-white">28/06/2023</p>
            </div>
            <p class="mt-3 text-lg md:text-xl text-blue-800 font-bold cursor-pointer">{{ items.title }}</p>
          </div>
        </div>
      </div>
    </div>
    <div class="flex justify-center">
      <button class="text-blue-900 bg-white border-1px border-blue font-bold text-center p-2 rd-20px w-150px">XEM THÊM</button>
    </div>
  </div>
</template>

<script setup>
const newsItems = [
  {
    image: "/11.png",
    date: "07:30 19-08-2023",
    title: "5 TRƯỜNG ĐÀO TẠO KHOA HỌC MÁY TÍNH TỐT NHẤT THẾ GIỚI",
  },
  {
    image: "/13.png",
    date: "07:30 19-08-2023",
    title: "5 trường Đại học đào tạo khoa học máy tính tốt nhất thế giới",
  },
  {
    image: "/14.png",
    date: "07:30 19-08-2023",
    title: "5 trường Đại học đào tạo khoa học máy tính tốt nhất thế giới",
  },
  {
    image: "/15.png",
    date: "07:30 19-08-2023",
    title: "5 trường Đại học đào tạo khoa học máy tính tốt nhất thế giới",
  },
]
</script>
