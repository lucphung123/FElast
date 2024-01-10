<template>
  <div class="w-full lg:px-0 flex flex-col">
    <div class="relative mt-60 md:mt-20 lg:mt-36 xl:mt-125 mb-0 md:mb-50 w-full">
      <div class="absolute h-170 w-screen left-1/2 -translate-x-1/2 -translate-y-full md:mt-43 bg-[url(/bg-banner.jpg)] bg-bottom bg-cover">
        <div class="w-full mx-auto flex items-center justify-between">
          <Slide />
        </div>
      </div>
    </div>
    <div class="flex items-center py-10">
      <div class="i-mdi:bookmark-outline text-4xl bg-blue-900"></div>
      <div class="text-3xl text-#004390 font-700">SÁCH NHIỀU NGƯỜI ĐỌC</div>
    </div>
    <div class="mb-10 w-full">
      <div class="relative w-80 bg-gray-200 rounded">
        <div class="absolute h-full transition-all duration-400 ease-in-out rounded-[5px] left-0 top-0 bg-#004390 text-white" :style="{ width: sliderWidth, left: sliderLeft }"></div>
        <div v-for="(tab, index) in tabs" :key="index" class="relative inline-block h-full text-7 text-center items-center cursor-pointer transition-all duration-300 ease-in-out rounded px-2 py-2 mr-0.5 hover:(bg-#004390 !text-white)" :class="activeTab === tab.id ? '!text-white' : ''" @click="moveSlider($event, index)">
          {{ tab.label }}
        </div>
      </div>
    </div>
    <News />

  </div>
</template>

<script setup>

const persentwidth = computed(() => {
  return `${(offWidth.value / 4800) * 100}%`
})

const offWidth = ref(0)
const sliderWidth = ref("90px")
const sliderLeft = ref("0px")
const tabs = [
  { id: "0", label: "Tất cả" },
  { id: "1", label: "Trẻ em" },
  { id: "2", label: "Người lớn" },
]
const activeTab = ref("0")
function moveSlider(event, index) {
  activeTab.value = tabs[index].id
  const tabWidth = event.currentTarget.offsetWidth
  sliderWidth.value = `${tabWidth}px`
  const tabLeft = event.currentTarget.offsetLeft
  sliderLeft.value = `${tabLeft}px`
}
function isActiveTab(index) {
  return activeTab.value === tabs[index].id
}
</script>
