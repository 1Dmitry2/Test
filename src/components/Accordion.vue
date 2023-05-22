<script setup lang="ts">
let truePlaceholder = "Да"
let falsePlaceholder = "Нет"
</script>

<script lang="ts">

export default {
  props: ['title', 'items'],

  data() {
    return {
      accordionOpen: false
    }
  },

  methods: {
    toggleOpen() {
      this.accordionOpen = !this.accordionOpen
      console.log(this.accordionOpen)
    }
}
}
</script>

<template>
  <div class="">
    <div class="flex justify-between cursor-pointer w-96" @click="toggleOpen">
      <h3 class="text-left font-semibold pb-2">{{ title }}</h3>
      <img src="/arrow.svg" class="" alt="">
    </div>

    <div v-for="item in items" class="transition-all" :class="accordionOpen ? 'opacity-0' : 'opacity-100'">
      <div class="grid grid-cols-2 gap-5 text-left pb-2" :class="{ hidden : accordionOpen}">
        <div>{{ item.name }}</div>
        <div>{{ typeof(item.value) == 'boolean' ? 
        item.value ? truePlaceholder : falsePlaceholder : (item.value2 ? 
        item.value1 + ' / ' + item.value2 + " " + item.unit : item.value1 + " " + item.unit) }}</div>
      </div>
      <hr />
    </div>
    <hr/>
  </div>
</template>

<style scoped>

</style>
