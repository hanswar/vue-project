<template>
    <div>
      <label><input type="radio" :value="radioValue1" v-model="picked"> 서울</label>
      <label><input type="radio" :value="radioValue2" v-model="picked"> 부산</label>
      <label><input type="radio" :value="radioValue3" v-model="picked"> 제주</label>
      <br>
      <span>선택한 키: {{ picked.key }}</span>
      <br>
      <span>선택한 지역: {{ picked.value }}</span>
    </div>
  </template>
  
  <script>
  export default {
      data() {
          return {
            picked: '',
            radioValue1: {key:1, value:'서울'},
            radioValue2: {key:2, value:'부산'},
            radioValue3: {key:3, value:'제주'},
          }
      }
  }
  </script>
  
  <style>
  
  </style>