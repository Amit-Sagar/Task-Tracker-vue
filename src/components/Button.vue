<template>
  <button @click="onClick()" class="btn" :style="{ background: color }">
    {{ text }}
  </button>
</template>
<script>
export default {
  name: "Button",
  methods: {
    onClick() {
        this.$emit('btn-click')
    },
  },
  props: {
    text: String,
    color: String,
  },
};
</script>
