<script>
export default {
  props: ["legend", "urlImage"],
};
</script>
<template>
  <div id="img-div">
    <figure>
      <img id="image" :src="urlImage" alt="Pucca and Garu" />
      <figcaption class="description">{{ legend }}</figcaption>
    </figure>
  </div>
</template>
<style >
#img-div {
  display: flex;
  flex-direction: column;
}
#image {
  margin-top: 2rem;
  width: 100%;
  border: 1px solid black;
  border-radius: 0.5rem;
  border-width: 2px;
  padding: 1rem;
}
.description {
  text-align: center;
  margin-bottom: 2rem;
  color: red;
  background-color: black;
  font-weight: bold;
}
</style>