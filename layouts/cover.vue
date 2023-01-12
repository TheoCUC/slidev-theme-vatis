<template>
  <div class="h-full flex items-center">
    <img src="/vatis.png" class="w-30 absolute top-5 left-5">
    <img src="/cuclogo.png" class="w-60 absolute top-5 right-5">
    <div class="bg-[#052780] w-full ">
      <div class="slidev-layout cover my-auto text-white">
        <slot />
      </div>
    </div>
  </div>
</template>
