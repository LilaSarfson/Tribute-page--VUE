<script>
export default {
  props: ["items"],
};
</script>
<template>
  <ul class="ul-list">
    <li v-for="datos in items" :key="datos.id">
      {{ datos.description }}
    </li>
  </ul>
</template>
<style>
.ul-list {
  margin-top: 1.5rem;
  display: flex;
  flex-direction: column;
  gap: 10px;
  text-align: start;
}
</style>