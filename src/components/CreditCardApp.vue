<template>
    <div>
        <div class="flex justify-center items-center mb-16 text-blue-600 text-lg">
            <h1>Credit Card Application</h1>
        </div>
        <div>
            <choose-credit-card-block-vue />
            <FAQBlockVue></FAQBlockVue>
        </div>

    </div>
</template>

<script setup lang="ts">
import ChooseCreditCardBlockVue from './ChooseCreditCardBlock.vue';
import FAQBlockVue from './FAQBlock.vue';
</script>

<style scoped>
</style>