<template>
  <div class="component">
    <img class="component__image" :src="photoLogsData.imageUrl" :alt="photoLogsData.title" />
    <div class="component__details">
      <div class="component__title">
        <p>{{ photoLogsData.title }}</p>
      </div>
      <div class="component__author">
        <p>{{ photoLogsData.author }}</p>
      </div>
      <div class="component__source">
        <a :href="photoLogsData.sourceLink">{{ photoLogsData.websiteName }}</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {

    }
  },
  props: ["photoLogsData"],
}
</script>

<style scoped>
.component {
  border: solid 1.5px #000;
  border-radius: 10px;
  margin: 8rem auto;
  padding: 3rem;
  max-width: 1200px;
  /* height: 600px; */
}

.component__img {
  object-fit: cover;
  width: 100%;
  /* height: 60%; */
  border-radius: 10px;
}

/* .component__details {
  display: flex;
  justify-content: space-between;
  flex-direction: column;
  padding: 2rem;
  height: 30%;
} */

/* .component__title {
  font-size: 4rem;
  display: flex;
  justify-content: center;
}

.component__actions {
  display: flex;
  justify-content: space-between;
  align-items: center;
} */
</style>