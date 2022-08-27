<script setup>
    import {useCounterStore} from '@/store/general';
    import { storeToRefs } from 'pinia'

    const store = useCounterStore()
    const {count} = storeToRefs(store)

    const { increment } = store

</script>

<template >
  <h1 class="text-green-600 uppercase text-4xl font-bold mb-16">
    Vue3 starter
  </h1>

  <h2 class="text-xl font-bold">
    Includes:
  </h2>

  <div class="flex">
    <a href="https://vitejs.dev" target="_blank">
      <img src="./../assets/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./../assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
    <a href="https://vuejsforge.com/" target="_blank">
      <img src="./../assets/pinia.svg" class="logo pinia" alt="Pinia logo" />
    </a>
    <a href="https://tailwindcss.com/" target="_blank">
      <img src="./../assets/tailwind.png" class="logo tailwind" alt="Tailwind logo" />
    </a>
  </div>

  <ul class="mb-8">
    <li>Vite</li>
    <li>Pinia</li>
    <li>Vue router</li>
    <li>Tailwindcss</li>
  </ul>



  <h2>Counter: {{count}}</h2>
  <button @click="increment">Increase counter</button>

</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}

.logo.pinia:hover {
  filter: drop-shadow(0 0 2em rgba(246, 216, 68, 0.67));
}
.logo.tailwind:hover {
  filter: drop-shadow(0 0 2em rgba(52, 225, 241, 0.67));
}
</style>
