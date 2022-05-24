<template>
  <div>
    <ul>
      <item v-for="item in items" :key="item.index">{{ item }}</item>
    </ul>
  </div>
</template>

<script>
import Item from './Item.vue';

export default {
  components: {
    Item,
  },
  data() {
    return {
      items: ['아이템1', '아이템2', '아이템3', '아이템4', '아이템5']
    }
  },
}
</script>