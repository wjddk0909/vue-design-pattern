<template>
  <div>
    <ul>
      <li v-for="item in items" :key="item.index">
        {{ item }}
      </li>
    </ul>
    <button @click="$emit('renew')">renew items</button>
  </div>
</template>

<script>
export default {
  props: {
    items: {
      type: Array, // Array로만 들어와야 함
      required: true, // 필수값이라는 뜻
    },
  },
}
</script>