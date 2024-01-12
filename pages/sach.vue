<template>
  <div class="py-10">
    <div class="flex gap-10">
      <img class="w-30%" src="/11.png" alt="" />
      <div class="w-40%">
        <div class="pb-5 font-bold text-7">Tên sách</div>
        <hr />
        <div class="py-2 text-5 text-gray">Tên tác giả</div>
        <div class="text-7 py-5 text-#004390 font-bold">100.000đ</div>
        <button class="text-white bg-#004390 rounded-full h-40px w-130px font-bold text-sm border-none hover:(bg-#f1b821 text-black) mr-10 mt-10 cursor-pointer">Mua ngay</button>
        <button class="text-#004390 rounded-full h-40px w-170px font-bold text-sm border-none hover:(bg-#f1b821 text-black) cursor-pointer">Thêm vào giỏ hàng</button>
      </div>
      <div class="w-30%">
        <div class="flex items-center gap-5 bg-gray-200 p-2 mb-1">
          <img src="/policy-1.png" alt="" />
          <p>Giao hàng toàn quốc</p>
        </div>
        <div class="flex items-center gap-5 bg-gray-200 p-2 mb-1">
          <img src="/policy-2.png" alt="" />
          <p>Phương thức thanh toán</p>
        </div>
        <div class="flex items-center gap-5 bg-gray-200 p-2 mb-1">
          <img src="/policy-3.png" alt="" />
          <p>Phương thức đổi trả</p>
        </div>
        <div class="flex items-center gap-5 bg-gray-200 p-2">
          <img src="/policy-4.png" alt="" />
          <p>Hotline: 0987.654.321</p>
        </div>
      </div>
    </div>
    <div class="mt-10 w-70%">
      <n-tabs type="segment" animated>
        <n-tab-pane name="Chi tiết sản phẩm" tab="Chi tiết sản phẩm">
          <p class="">Chưa có thông số cho sản phẩm này</p>
        </n-tab-pane>
        <n-tab-pane name="Mô tả Sản phẩm" tab="Mô tả Sản phẩm">
          <p class="">Chưa có thông số cho sản phẩm này</p>
        </n-tab-pane>
        <n-tab-pane name="Đánh giá sản phẩm" tab="Đánh giá sản phẩm">
          <div class="flex items-center gap-5">
            <p class="">Hãy để lại đánh giá cho chúng tôi :</p>
            <n-rate size="large" />
          </div>
        </n-tab-pane>
      </n-tabs>
    </div>
  </div>
</template>

<script setup></script>
