<template>
    <div>
        <img src="/cuc.png" class="w-15 left-5 top-3 absolute">
        <img src="/vatisBar.png" class="mt-0" />
        <div class="slidev-layout default w-full">
            <div class="text-white text-4xl absolute top-6 left-0 mx-auto w-full text-center font-semibold">目录</div>
        </div>
        <div class="max-h-80 flex flex-col flex-wrap content-center justify-center gap-x-5">
            <div v-for="(item, index) in $slidev.configs.contents">
                <div class="flex my-2">
                    <div
                        class="bg-[#002e57] w-10 h-15 text-center text-4xl items-center justify-center text-white flex">
                        {{ index + 1 }}
                    </div>
                    <div class="flex mx-1 px-2 bg-[#004c8d] h-15 w-85 text-2xl text-white  items-center ">{{ item }}
                    </div>
                </div>
            </div>

        </div>
        <img src="/bottomBar.png" class="absolute bottom-0">
    </div>
</template>