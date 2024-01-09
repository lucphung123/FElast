<template>
  <div class="bg-white w30% h-screen ml35% shadow">
    <div class="ml15%">
      <img
        class="w40% ml20%"
        src="https://images.glints.com/unsafe/glints-dashboard.s3.amazonaws.com/company-banner-pic/d3a7e705efc2eb296bcfe869ceae5b57.jpg"
        alt=""
      />
      <h3>Đăng kí tài khoản</h3>
      <p>Nhập thông tin để đăng kí tài khoản.</p>
      <p class="font-bold">Họ tên</p>
      <input
        class="w80% h8 border-1px rd-1 opacity-70%"
        type="text"
        name="name"
        placeholder="Nhập họ tên của bạn"
      />
      <p class="font-bold">Địa chỉ Email</p>
      <input
        class="w80% h8 border-1px rd-1 opacity-70%"
        type="text"
        name="email"
        placeholder="Nhập địa chỉ Email"
      />
      <p class="font-bold">Mật khẩu</p>
      <input
        class="w80% h8 border-1px rd-1 opacity-70%"
        type="password"
        name="password"
        placeholder="Nhập mật khẩu"
      />

      <p class="font-bold">Số điện thoại</p>
      <input
        class="w80% h8 border-1px rd-1 opacity-70%"
        type="number"
        name="phone"
        placeholder="Nhập số điện thoại"
      /><br />
      <br />
      <button
        class="w81.5% h8 border-1px rd-1 bg-#1C00C2 border-white font-bold text-white"
        @click="handleRegister"
      >
        Hoàn tất đăng kí
      </button>
      <p class="ml24%">Hoặc đăng nhập với</p>
      <div class="flex">
        <button
          class="i-mdi:facebook text-xl bg-#1C00C2 ml10% cursor-pointer"
        ></button>
        <button
          class="i-mdi:google text-xl bg-red cursor-pointer ml50%"
        ></button>
      </div>
      <div class="flex gap1 items-center">
        <p>Bạn đã có tài khoản ?</p>
        <nuxt-link to="./login" class="decoration-none font-bold"
          >Quay lại trang đăng nhập</nuxt-link
        >
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const handleRegister = () => {
  // Lấy giá trị từ các trường nhập liệu
  const name = nameInput.value;
  const email = emailInput.value;
  const password = passwordInput.value;
  const phone = phoneInput.value;

  // Lưu thông tin vào localStorage
  localStorage.setItem("name", name);
  localStorage.setItem("email", email);
  localStorage.setItem("password", password);
  localStorage.setItem("phone", phone);
};

// Sử dụng ref để tham chiếu đến các trường nhập liệu
const nameInput = ref(null);
const emailInput = ref(null);
const passwordInput = ref(null);
const phoneInput = ref(null);
</script>
