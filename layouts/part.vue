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
    <div>
        <img src="https://isaacpic-1305775614.cos.ap-beijing.myqcloud.com/uPic/vatis.png" class="w-30 m-5 absolute top-0 right-0">
        <div>Part {{ id }}</div>
        <div class="slidev-layout intro h-1/4 my-50 bg-[#052780] text-white font-bold z-100" absolute top-60>
            <div class="my-auto z-100">
                <h1>{{nummap[id]}}、{{ $slidev.configs.contents[id-1] }}</h1>
            </div>
        </div>
        <div class="bg-[#e4e4e4] w-2/5 h-56 absolute top-0 left-0 z-10"></div>
        <div class="bg-[#e4e4e4] w-1/3 h-53 absolute bottom-0 right-0 z-10"></div>

    </div>
</template>
