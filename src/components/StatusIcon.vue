<template>
  <i class="icon" :class="{ connected: connected }"></i>
</template>

<script>
export default {
  name: "StatusIcon",
  props: {
    connected: Boolean,
  },
};
</script>

<style scoped>
.icon {
    height: 8px;
    width: 8px;
    border-radius: 50%;
    display: inline-block;
    background-color: #5f6368;
    margin-right: 6px;
}

.icon.connected {
    background-color: #34a853;
}
</style>
