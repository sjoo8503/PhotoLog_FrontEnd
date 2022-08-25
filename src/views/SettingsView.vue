<template>
  <form class="form" action="">
    <h2>Add Photo</h2>
    <div>
      <input class="author" type="text" placeholder="Author Name">
      <input class="post-title" type="text" placeholder="Post Title">
      <input class="image-url" type="text" placeholder="Image URL">
      <input class="source" type="text" placeholder="Source">
      <input class="source-url" type="text" placeholder="Source URL">
      <button class="add-btn">Add</button>
    </div>
  </form>

  <div class="search">
    <input class="search__item" type="text" placeholder="Search 🔎">
  </div>

  <div class="list-menu">
    <p>Image</p>
    <p>Details</p>
    <p>Actions</p>
  </div>
  <div>
    <setting-item></setting-item>
  </div>
</template>

<script>
import SettingItem from "../components/SettingItem.vue";
export default {
  data() {
    return {

    }
  },
  components: {
    SettingItem,
  }
}
</script>

<style scoped>
form {
  margin: 5rem 5rem 0;
}

form div {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

form h2 {
  font-size: 2.5rem;
}

.add-btn {
  padding: 1rem 4rem;
  text-transform: uppercase;
  letter-spacing: 0.1rem;
  border: solid 1px #255fb7;
  border-radius: 10px;
  font-weight: 700;
  background-color: #255fb7;
  color: #fff;
}

.search {
  margin: 5rem 5rem 0;

}

.list-menu {
  display: flex;
  justify-content: space-around;
  align-items: center;
  background-color: lightgrey;
  border-radius: 10px;
  font-size: 2.5rem;
  margin: 5rem 5rem 0;
  padding: 2rem;
}
</style>