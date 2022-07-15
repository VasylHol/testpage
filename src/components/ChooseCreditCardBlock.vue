<template>
    <div class="flex mt-8">
        <div class="bg-indigo-200 credit-card-block rounded ml-4 box-border">
            <div class="ml-8 pt-4 pb-2">
                <p class="text-left">
                    Which type of credit card do you want?
                </p>
            </div>
            <div class="flex justify-center">
                <CreditCardVue class="mr-2">
                    <template #credit-card-name>
                        Visa Lifestyle Plus
                    </template>
                    <template #credit-card-features>
                        <div v-for="item in items" :key="item.id"
                            class="flex flex-col justify-center mr-2 bg-indigo-100 w-1/3 h-28 rounded">
                            <b>{{ item.num }}</b>
                            {{ item.text }}
                        </div>
                    </template>
                    <template #credit-card-image> <img width="200" height="100" src="@/assets/goldvisa.jpg"
                            alt=""></template>
                    <template #credit-card-text>
                        <p>If you are looking for more freedom in your credit card, our low rate and no annual free Visa
                            Lifestyle Plus credit card may be for you</p>
                    </template>
                </CreditCardVue>
                <CreditCardVue>
                    <template #credit-card-name>
                        Visa Lifestyle Plus
                    </template>
                    <template #credit-card-features>
                        <div v-for="item in items" :key="item.id"
                            class="flex flex-col justify-center mr-2 bg-indigo-100 w-1/3 h-28 rounded">
                            <b>{{ item.num }}</b>
                            {{ item.text }}
                        </div>
                    </template>
                    <template #credit-card-image> <img width="200" height="100" src="@/assets/blackvisa.jpg"
                            alt=""></template>
                    <template #credit-card-text>
                        <p>If you are looking for more freedom in your credit card, our low rate and no annual free Visa
                            Lifestyle Plus credit card may be for you</p>
                    </template>
                </CreditCardVue>
            </div>
        </div>
        <div class=" flex flex-col faq ml-16 text-lg">
            <p class="border-b-2 border-b-slate-200 text-left pb-4">FAQs</p>
            <div class="flex items-center justify-center">
                <QuestionMarkCircleIcon class="h-5 w-5 mt-4 mr-4" />
                <select class="text-sm mt-4 w-[700px]">
                    <option value="0">Lorem ipsum</option>
                </select>
            </div>
            <div class="w-[500px] text-left text-sm text-slate-400 ml-12 mt-4 font-normal">
                <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Tempore iusto sapiente officiis
                        distinctio
                        nobis itaque harum, fugiat aspernatur illo accusamus ad, suscipit blanditiis quae, deserunt modi
                        debitis. Nihil, deleniti odit.

                </p>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';
import CreditCardVue from './CreditCard.vue';
import { QuestionMarkCircleIcon } from "@heroicons/vue/outline"
const items = ref([{ id: 4234234, num: '$0', text: 'Annual fee' }, { id: 464534234, num: 'xx%', text: 'Purchase rate' }, { id: 432775234, num: '100', text: 'Interest free days' },])
</script>

<style scoped>
.credit-card-block {
    width: 45%;
    height: 500px;
}

.faq {
    width: 30%;
}
</style>