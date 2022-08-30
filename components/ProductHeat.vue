<script setup>
defineProps({
  heatLevel: String,
});
const heatMap = {
  Hot: "🔥🔥🔥",
  Medium: "🔥🔥",
  Mild: "🔥",
};
</script>
<template>
  <span>
    {{ heatLevel[0] ? heatMap[heatLevel] : "" }}
  </span>
</template>
