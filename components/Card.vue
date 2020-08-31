<template>
  <div class="card">
    <img :src="img">
    <div class="inner">
      <h1>{{ title }}</h1>
      <p>
        <span class="tag" v-for="tag in tags" :key="tag">
          <span>#{{ tag }}</span>
        </span>
      </p>
      <p>{{ description }}</p>
      <a :href="link">Link ></a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    title: String,
    tags: Array,
    description: String,
    link: String,
    img: Boolean,
    src: String
  },
  data() {
    return {
      img: this.img
    }
  }
}
</script>

<style scoped>
.card {
  border-radius: 10px;
  margin-bottom: 1rem;
  background: #bbffc6 none repeat scroll 0% 0%;
  color: #000; }
img {
  display: block;
  max-width: 50%;
  border-radius: 5px 5px 0px 0px; }
div {
  padding: 10px; }
h1 {
  font-size: 35px;
  margin: 16px -3px; }
span {
  margin-right: 5px; }
p {
  font-size: 25px;
    margin: 10px 0; }
a {
  text-decoration: none;
  color: #000;
  font-size: 20px; }
</style>