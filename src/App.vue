
<template>
    <div class="card flex justify-content-center">
        <label for="calendar-12h" class="font-bold block mb-2"> 12h Format </label>
        <Calendar
            id="calendar-12h"
            v-model="datetime12h"
            showTime hourFormat="12"
            showIcon
            :pt="{
                input: { class: 'w-16rem' },
                dropdownButton: {
                    root: { class: 'bg-teal-500 border-teal-500' }
                },
                ampm: {

                }
            }"
        />
    </div>
</template>


<script setup>
import { ref } from "vue";

const datetime12h = ref();
const pm = ref();
</script>