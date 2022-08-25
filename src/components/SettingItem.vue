<template>
  <div class="component">
    <img class="component__img" src="../assets/img/cristian-castillo-73pyV0JJOmE-unsplash.jpg" alt="dog">
    <div class="component__details">
      <p>Author: Cristian Castillo</p>
      <p>Title: Running Puppy</p>
      <p>Source: Upsplash.com</p>
      <a>Source URL: https://unsplash.com/photos/73pyV0JJOmE</a>
    </div>
    <div class="component__actions">
      <a href=""><i class="fas fa-pen"></i></a>
      <a href=""><i class="fas fa-eye"></i></a>
      <a href=""><i class="fas fa-trash"></i></a>
    </div>
  </div>
  <div class="component">
    <img class="component__img" src="../assets/img/cristian-castillo-73pyV0JJOmE-unsplash.jpg" alt="dog">
    <div class="component__details">
      <p>Author: Cristian Castillo</p>
      <p>Title: Running Puppy</p>
      <p>Source: Upsplash.com</p>
      <a>Source URL: https://unsplash.com/photos/73pyV0JJOmE</a>
    </div>
    <div class="component__actions">
      <a href=""><i class="fas fa-pen"></i></a>
      <a href=""><i class="fas fa-eye"></i></a>
      <a href=""><i class="fas fa-trash"></i></a>
    </div>
  </div>
  <div class="component">
    <img class="component__img" src="../assets/img/cristian-castillo-73pyV0JJOmE-unsplash.jpg" alt="dog">
    <div class="component__details">
      <p>Author: Cristian Castillo</p>
      <p>Title: Running Puppy</p>
      <p>Source: Upsplash.com</p>
      <a>Source URL: https://unsplash.com/photos/73pyV0JJOmE</a>
    </div>
    <div class="component__actions">
      <a href=""><i class="fas fa-pen"></i></a>
      <a href=""><i class="fas fa-eye"></i></a>
      <a href=""><i class="fas fa-trash"></i></a>
    </div>
  </div>

</template>

<script>

</script>

<style scoped>
.component {
  display: flex;
  align-items: center;
  justify-content: space-between;
  border: solid 1.5px #000;
  border-radius: 10px;
  margin: 8rem auto;
  padding: 3rem;
  max-width: 1500px;
  /* height: 600px; */
}

.component__img {
  /* object-fit: cover; */
  width: 25%;
  /* height: 60%; */
  border-radius: 10px;
}

.component__details,
.component__actions {
  font-size: 3.5rem;
}

.component__details * {
  margin-bottom: 1.5rem;
}

.component__actions a:not(:first-of-type) {
  margin-left: 5rem;
}

.component__actions a {
  color: #255fb7;
}
</style>