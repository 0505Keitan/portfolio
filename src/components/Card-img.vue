<template>
  <div class="card-container">
    <img :src="img">
    <div class="inner">
      <h1>{{ title }}</h1>
      <p>
        <span class="tag" v-for="item in items" :key="item">
          <span>#{{ item }}</span>
        </span>
      </p>
      <p>{{ description }}</p>
      <a :href="link">Link ></a>
    </div>
  </div>
</template>

<script>
export default {
  props: ["title", "tags", "description", "link", "img"],
  data: function() {
    return {
      items: this.tags.split(",")
    }
  }
}
</script>

<style scoped>
.card-container {
  border-radius: 10px;
  margin-bottom: 1rem;
  background: #00510d none repeat scroll 0% 0%;
  color: #E3E3E3;
  display: inline-block;
  width: 100%;
  margin-right: 10px; }
img {
  display: block;
  max-width: 100%;
  border-radius: 5px 5px 0px 0px; }
div {
  padding: 10px; }
h1 {
  margin-top: 0px;
  font-size: 30px;
  margin: 5px 0px; }
span {
  font-size: 15px;
  margin-right: 5px; }
a {
  text-decoration: none;
  color: #E3E3E3; }
</style>