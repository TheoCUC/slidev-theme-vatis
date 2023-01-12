<script>
import { defineComponent } from "vue";

export default defineComponent({
    props: {
        id: {
            type: Number,
            required: true,
        },
    },
});
</script>
<template>
    <div>
        <img src="/cuc.png" class="w-15 absolute top-2 left-5" />
        <img src="/vatisBar.png" class="mt-0 visible" />
        <div class="text-white text-4xl absolute top-6 left-0 mx-auto w-full text-center font-semibold">
            {{ $slidev.configs.contents[id - 1] }}
        </div>
        <div class="slidev-layout default w-full relative pt-6 px-15">
            <div class="my-auto">
                <slot />
            </div>
        </div>
        <div class="z-10 absolute bottom-2 left-8 text-white font-black">
            {{ $slidev.nav.currentPage }}
        </div>
        <img src="/bottomBar.png" class="absolute inset-x-0 bottom-0" />
    </div>
</template>
