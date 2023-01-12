<script>
import { defineComponent } from "vue";

export default defineComponent({
    props: {
        id: {
            type: Number,
            required: true,
        },
    },
    data() {
        return {
            nummap: { 1: '一', 2: '二', 3: '三', 4: '四', 5: '五', 6: '六', 7: '七', 8: '八', 9: '九', 10: '十' }
        }
    },
});
</script>

<template>
    <div class="h-full flex items-center">
        <img src="/vatis.png" class="w-30 m-5 absolute top-0 right-0">
        <div class="bg-[#e4e4e4] w-2/5 h-56 absolute top-0 left-0 z-0"></div>
        <div class="bg-[#e4e4e4] w-1/3 h-53 absolute bottom-0 right-0"></div>
        <div class="w-full z-10">
            <div class="slidev-layout intro bg-[#052780] text-white font-bold">
                <div class="my-auto z-3">
                    <h1>{{ nummap[id]}}、{{ $slidev.configs.contents[id - 1] }}</h1>
                </div>
            </div>
        </div>
    </div>
</template>
