<script>
export default {
  props: ["years", "text"],
};
</script>
<template>
  <li>
    <span>{{ years }}</span>
    <span>{{ text }}</span>
  </li>
</template>