<template>
  <div class="flex justify-center items-center h-screen">
    <div class="flex items-center mr-50">
      <img class="w-12 h-12 mr-2" src="./ladipage.png" alt="Ladipage logo" />
      <h1 class="text-2xl font-bold">iPages</h1>
    </div>
    <div class="bg-white rounded-lg shadow-lg p-6">
      <h2>Đăng nhập</h2>
      <p class="text-center">Nhập thông tin để đăng nhập vào tài khoản</p>
      <h3>Địa chỉ Email</h3>
      <n-input
        type="text"
        placeholder="Nhập địa chỉ Email"
        class="w-full mb-2"
      />
      <h3>Mật khẩu</h3>
      <n-input placeholder="Nhập mật khẩu" type="password" class="w-full mb-2" />
      <p>Quên mật khẩu?</p>
      <n-button class="w-full">Đăng nhập</n-button>
      <p class="text-center mt-4">Hoặc đăng nhập với</p>
      <i class="i-facebook text-2xl text-blue-500 cursor-pointer"></i>
    </div>
  </div>
</template>
