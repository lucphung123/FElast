<template>
  <div class="fixed bg-white w100% left-0 top-0 flex items-center h12%">
    <div class="flex items-center">
      <img
        class="w15%"
        src="https://images.glints.com/unsafe/glints-dashboard.s3.amazonaws.com/company-banner-pic/d3a7e705efc2eb296bcfe869ceae5b57.jpg"
        alt=""
      />

      <div class="flex gap10 ml5%">
        <p class="text-xl">Giải pháp</p>
        <p class="text-xl">Công cụ</p>
        <p class="font-bold text-xl">Bảng giá</p>
        <p class="text-xl">Tài liệu</p>
      </div>
    </div>
    <div class="flex gap3 mr40">
      <nuxt-link to="./login"
        ><button
          class="cursor-pointer hover-bg-#0000FF hover-text-white border-blue border-1px text-blue bg-white w30 h10 rd-5"
        >
          Đăng Nhập
        </button></nuxt-link
      >
      <nuxt-link to="./register"
        ><button
          class="cursor-pointer bg-#0000FF text-white w30 h10 border-none rd-5"
        >
          Đăng kí
        </button></nuxt-link
      >
    </div>
  </div>
  <hr class="mt6%" />
  <div>
    <p class="flex justify-center font-1000 text-2xl text-blue mt10%">
      Landing Page Platform
    </p>
    <div>
      <main class="container">
        <p class="flex justify-center text-5xl font-1000 text-#0000FF mt--1">
          Nền tảng landing page chuyển đổi cao
        </p>

        <div
          class="flex items-center justify-center text-5xl font-1000 text-#0000FF mt--4%"
        >
          <p>cho các hoạt động</p>
          <section class="animation">
            <div class="first text-#FF0000"><div>Quảng Cáo</div></div>
            <div class="second text-#FF0000"><div>Bán Hàng</div></div>
            <div class="third text-#FF0000"><div>Marketing</div></div>
          </section>
        </div>
      </main>
    </div>
    <div class="mt--39%">
      <p class="flex justify-center text-xl font-500">
        Hiện thực hoá các mục tiêu bán hàng và tối đa hoá chuyển đổi quảng cáo
      </p>
      <p class="flex justify-center text-xl font-500">
        Không cần lập trình • Miễn phí hosting • Bảo mật dữ liệu
      </p>
    </div>
  </div>
  <div class="flex justify-center mt3% gap3% ">
    <button
      class="cursor-pointer hover-bg-#0000FF hover-text-white border-blue border-1px text-#0000FF bg-white w50 h10 rd-5"
    >
      Nhận tư vấn qua Livechat
    </button>
    <button
      class="cursor-pointer bg-#0000FF text-white w50 h10 border-none rd-5"
    >
      Sử dụng miễn phí ngay
    </button>
  </div>
</template>

<script setup>


</script>
<style>
p {
  text-shadow: 0 0 7px rgba(255, 255, 255, 0.3),
    0 0 3px rgba(255, 255, 255, 0.3);
}
.container {
  font-size: 2.26rem;
  text-transform: uppercase;
  height: 100vh;
  justify-items: center;
  align-items: center;
  justify-content: center;
}

.animation {
  height: 50px;
  overflow: hidden;
  margin-left: 1rem;
}

.animation > div > div {
  height: 2.81rem;
  margin-bottom: 2.81rem;
  display: inline-block;
}

.animation div:first-child {
  animation: text-animation 6s infinite;
}

.first div {
  background-color: #fcfdfe;
}
.second div {
  background-color: #fefdfa;
}
.third div {
  background-color: #fefcfd;
}

@keyframes text-animation {
  0% {
    margin-top: 0;
  }
  10% {
    margin-top: 0;
  }
  20% {
    margin-top: -5.62rem;
  }
  30% {
    margin-top: -5.62rem;
  }
  40% {
    margin-top: -11.24rem;
  }
  60% {
    margin-top: -11.24rem;
  }
  70% {
    margin-top: -5.62rem;
  }
  80% {
    margin-top: -5.62rem;
  }
  90% {
    margin-top: 0;
  }
  100% {
    margin-top: 0;
  }
}
</style>
