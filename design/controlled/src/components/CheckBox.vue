<template>
  <!--  v-model input이벤트와 value값으로 조작 받을때 value로 받고 input을 올린다...?-->
  <input type="checkbox" :value="value" @click="toggleCheckBox">
</template>

<script>
export default {
  // props: ['checked'],
  // @input 이벤트
  // :value 값
  props: ['value'], // v-model이 일단은 value로 내려옴
  methods: {
    toggleCheckBox() {
      this.$emit('input', !this.value)
    }
  }
}
</script>