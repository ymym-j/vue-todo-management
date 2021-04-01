<template>
  <button type="button" class="list-group-item text-left" @click="click">{{ value }}</button>
</template>
<script>
export default {
  props: ['value'],
  methods: {
    click() {
      this.$emit('component-click');
    }
  }
};
</script>