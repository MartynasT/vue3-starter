<script setup>
import {useCounterStore} from '@/store/general';
import { storeToRefs } from 'pinia'

const store = useCounterStore()
const {count} = storeToRefs(store)

</script>

<template >
    <h1 class="text-green-600 uppercase text-4xl font-bold mb-16">
        About Page
    </h1>
    <h2>Counter: {{count}}</h2>

</template>
