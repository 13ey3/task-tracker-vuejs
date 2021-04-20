<template>
  <button @click="onClick()" :style="{ background: color }" class="btn">{{ btnName }}</button>
</template>

<script>
export default {
  name: "Button",
  props: {
    btnName: String,
    color: String,
  },
  methods: {
      onClick() {
          this.$emit('btn-click')
      }
  }
};
</script>
