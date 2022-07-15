<template>
    <div class="flex">
        <div class="bg-white py-2 px-4 border-2  border-slate-400 rounded-md">
            <p class="text-left text-base text-blue-600 mt-4 mb-4">
                <slot name="credit-card-name">test name</slot>
            </p>
            <div class="flex items-center justify-center">
                <slot name="credit-card-features">
                    <div>1</div>
                    <div>2</div>
                    <div>3</div>
                </slot>
            </div>
        <div class="flex mt-4">
            <div class="">
                <slot name="credit-card-image"> img</slot>
            </div>
            <div class="text-sm w-60 text-left ml-4 text-gray-400">
                <slot name="credit-card-text"> test text</slot>
            </div>
        </div>
        <div class="pt-4 mt-4 flex justify-between border-t-2 border-t-slate-200">
            <button class="py-4 px-12 bg-slate-200">
              Learn More  
            </button>
            <button class="bg-sky-300 py-4 px-16 ml-1">
                Next Steps
            </button>
        </div>
        </div>
    </div>
</template>

<script setup lang="ts">


</script>

<style scoped>
</style>