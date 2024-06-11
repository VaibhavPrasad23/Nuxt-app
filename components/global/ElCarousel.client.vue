<template>
    <carousel :items-to-show="5.5">
      <slide v-for="slide in 10" :key="slide">
        {{ slide }}
      </slide>
  
      <template #addons>
        <navigation />
        <pagination />
      </template>
    </carousel>
  </template>
  