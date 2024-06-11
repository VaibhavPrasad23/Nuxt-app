<template>
    <carousel :items-to-show="10">
      <slide v-for="slide in 10" :key="slide">
        <img :src="`/_nuxt/assets/${slide}.jpg`" />
        
      </slide>
  
      <template #addons>
        <navigation />
        <pagination />
      </template>
    </carousel>
  </template>
  

<style scoped>


section.carousel{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 600px;
    height: 300px;
    margin-left: 90px;
    background-color: #f9f9f9;
    border-radius: 4px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}
 </style>