<script setup lang="ts">
import Accordion from './components/Accordion.vue'
</script>

<template>
  <Accordion 
  title="Водоизмещение"
  :items="[
    {name: 'Судно порожнем', value1: '8 296.50', unit: 'T'},
    {name: 'Дедвейт', value1: '20 935.5', value2: '25 000', unit: 'T'},
    {name: 'Тру', value: true},
    {name: 'Фолз', value: false},
    {name: 'Водоизмещение', value1: '29 242.04', value2: '25 000', unit: 'T'},
    {name: 'Водоизмещение по ЛГМ', value1: '33 417', value2: '25 000', unit: 'T'},
    {name: 'Груз', value1: '19 401.6', value2: '43 554.7', unit: 'T'},
    {name: 'Жидкий балласт', value1: '0', value2: '11 147.59', unit: 'T'},
    {name: 'Тяжелое топливо', value1: '982.5', value2: '892.44', unit: 'T'},
    {name: 'Дизельное топливо', value1: '113.3', value2: '113.30', unit: 'T'},
    {name: 'Пресная вода', value1: '152.2', value2: '152.10', unit: 'T'},
    {name: 'Смазочное масло', value1: '37.89', value2: '42.10', unit: 'T'},
    {name: 'Постоянные нагрузки', value1: '45', unit: 'T'},
    ]" />
      <Accordion 
  title="Посадка судна"
  :items="[
    {name: 'Дифферент', value1: '-1.75', unit: 'м'},
    {name: 'Угол крена', value1: '0', unit: '°'},
    {name: 'Заглубление винта', value1: '99', unit: '%'},
    {name: 'Осадка носом', value1: '9.68', unit: 'м'},
    {name: 'Осадка кормой', value1: '8.8', unit: 'м'},
    {name: 'Осадка на миделе', value1: '9.67', unit: 'м'},
    {name: 'Средняя осадка', value1: '10.55', unit: 'м'},
    ]" />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
